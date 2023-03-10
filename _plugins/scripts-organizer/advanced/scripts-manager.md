---
title: 'Scripts Manager'
---

With this powerful feature, you will be able to enqueue and register scripts and styles and trigger them in the same way as any other code you are writing inside Scripts Organizer. dPlugins products work perfectly together and are cross-functional so what you register in Swiss Knife it will be visible here as well and vice versa. This feature is not for writing the code, it's for including libraries such as [GreenSock](https://greensock.com/) or [Bootstrap](https://getbootstrap.com/).

## How to use Scripts Manager Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/JmQumgVp2qQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Reusing Registered Scripts

<iframe width="560" height="315" src="https://www.youtube.com/embed/s4s8kHXRiN0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Enable Scripts manager

This feature is not enabled by default and you need to enable it manually. Go to Scripts Organizer in the admin menu and find the "Features" sub-menu. From there select "Enable Scripts Manager" and save changes. After you have saved the changes, reload the page in order to see the new sub-menu "Scripts Manager".

## Allow CSS/JS Uploads

WordPress by default does not allow uploading CSS or JavaScript files.

This feature is safe as it is in Admin only condition. Users need to be logged in as Admin in order to upload CSS and JS files.


![](../../img/advanced/Screenshot-2021-11-09-at-13.12.16.png)

## Add Script or Style

Once the feature is enabled open the sub-menu "Scripts Manager". Hit "+ Add New Script".

A new block will be displayed with several options.

![](../../img/advanced/add-new.png)

![](../../img/advanced/Screenshot-2021-11-09-at-13.16.52.png)

### Script Name

Use this field to describe your included file name.

### Script Type

Choose if the file you are including is JavaScript or CSS.

### Location

Choose if the file you are adding will be included in the Header (before opening body tag) or the Footer (before closing body tag ) of the website. For the best performance include CSS in the header and JavaScript in the footer.

### Include type

#### **Enqueue** 

Enqueued script will run on every page of the website.

#### **Register** 

Register script will be pre-loaded on the website but not injected into the page.

You will need to trigger it manually. This is good if you don't want to have the script on every page of the website.

To trigger the registered Script or Style go to Scripts inside code editor and under scripts manager settings select script. The script will be triggered based on the above-provided conditions.

### Frontend only

If this option is active this script will be available only for users who are not logged in. This is good if you don't want that script interfering with builders.

### Upload file (self-host) or paste CDN link

Here you can paste links from CDN or relative links from WordPress installation.

Besides pasting links you can self-host scripts by yourself as well. Press the "Up Arrow" icon and WordPress Media Library will be prompted. Drag and drop a file and the link will be autogenerated by WordPress.

#### **Note:** Upload Scripts and Styles is not allowed by default by WordPress.

To allow it go to the Features Sub-menu and activate: Allow CSS/JS Uploads. For best practices disable this feature after you upload needed scripts.

### Click to copy

This will generate a code that you can copy in PHP blocks and Enqueue (inject) script on only needed pages.

This option is available in edit script mode and when the script is collapsed.


![](../../img/advanced/Screenshot-2021-11-09-at-13.17.34.png)

![](../../img/advanced/Screenshot-2021-11-09-at-13.18.14.png)

## Integration with Oxygen Builder

<iframe width="560" height="315" src="https://www.youtube.com/embed/bBRw4uA4TU8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>