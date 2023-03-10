---
title: Bricks Builder
---

We have first-class support for [Bricks Builder](https://bricksbuilder.com/), a powerful page builder for WordPress.

## `SYNC_BREAKPOINT` placeholder

In the Bricks Builder [1.5.1](https://bricksbuilder.io/changelog/#v1.5.1) release, Bricks Builder introduced a new feature called "Custom Breakpoints" that allows you edit the default breakpoints, add your own custom breakpoints, set a different base breakpoint, and use a mobile-first design approach.

![Custom Breakpoints](/img/custom-breakpoints.png)

Winden provides a placeholder for the Bricks Builder custom breakpoints: `SYNC_BREAKPOINT`. You can use this placeholder in the "Tailwind Config" field on the Winden setting page and below the Settings tab that will be replaced with the actual breakpoint value.

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

```mdx-code-block
<Tabs>
<TabItem value="wp-content/uploads/winden/cdn.config.js">
```

```js
module.exports = {
  theme: {
    screens: {
      // highlight-next-line
      ...SYNC_BREAKPOINT
    },
    extend: {
      colors: {
        clifford: '#da373d',
      },
    },
  },
  plugins: [],
  corePlugins: {
    preflight: false,
  }
}
```

```mdx-code-block
</TabItem>
<TabItem value="Example Output">
```

```js
module.exports = {
  theme: {
    screens: {
      // highlight-start
      ...{
        "mobile_landscape": { "raw": "(max-width: 767px)" },
        "tablet_portrait": { "raw": "(min-width: 991px)" },
        "desktop": { "raw": "(min-width: 1279px)" },
        "mobile_portrait": { "raw": "(max-width: 478px)" }
      }
      // highlight-end
    },
    extend: {
      colors: {
        clifford: '#da373d',
      },
    },
  },
  plugins: [],
  corePlugins: {
    preflight: false,
  }
}
```

```mdx-code-block
</TabItem>
</Tabs>
```

To use the breakpoint on your class, you can use the "Key" of the breakpoint as the prefix of class, such as `mobile_landscape:text-center`, `tablet_portrait:bg-yellow-100`, and `desktop:p-4`.

We also provide `f!winden/builder/bricks/runtime:breakpoint_key` filter hook to change the default breakpoint key that will be used in the class name.

```php
<?php

add_filter('f!winden/builder/bricks/runtime:breakpoint_key', 'example_bricks_rename_breakpoint_key', 10);

function example_bricks_rename_breakpoint_key(string $key): string
{
    if ($key === 'mobile_portrait') {
        return 'mobile';
    } elseif ($key === 'mobile_landscape') {
        return 'mobile_l';
    } elseif ($key === 'tablet_portrait') {
        return 'tablet';
    }

    return $key;
}
```

Then you can use the new breakpoint key in your class name, such as `mobile:text-center`, `tablet:bg-yellow-100`, and `desktop:p-4`.