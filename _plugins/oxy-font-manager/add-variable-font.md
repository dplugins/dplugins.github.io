---
id: 29266
title: 'Add Variable Font'
date: '2022-03-10T19:11:18+00:00'
author: devusrmk
layout: oxy_font_manager
guid: 'https://docs.dplugins.com/?post_type=oxy_font_manager&#038;p=29266'
permalink: /oxy_font_manager/add-variable-font/
algolia_searchable_posts_records_count:
    - '1'
hide_title:
    - '0'
updated:
    - '0'
ct_other_template:
    - '0'
ct_template_archive_post_types_all:
    - ''
ct_template_categories:
    - 'a:0:{}'
ct_template_categories_all:
    - ''
ct_template_tags:
    - 'a:0:{}'
ct_template_tags_all:
    - ''
ct_template_custom_taxonomies:
    - 'a:0:{}'
ct_template_custom_taxonomies_all:
    - ''
ct_template_authors_archives_all:
    - ''
ct_template_index:
    - ''
ct_template_front_page:
    - ''
ct_template_blog_posts:
    - ''
ct_template_date_archive:
    - ''
ct_template_search_page:
    - ''
ct_template_inner_content:
    - ''
ct_template_404_page:
    - ''
ct_template_all_archives:
    - ''
ct_template_archive_among_taxonomies:
    - 'a:0:{}'
ct_template_apply_if_archive_among_taxonomies:
    - ''
ct_template_archive_post_types:
    - 'a:0:{}'
ct_template_apply_if_archive_among_cpt:
    - ''
ct_template_authors_archives:
    - 'a:0:{}'
ct_template_apply_if_archive_among_authors:
    - ''
ct_template_single_all:
    - ''
ct_template_post_types:
    - 'a:0:{}'
ct_template_exclude_ids:
    - ''
ct_template_include_ids:
    - ''
ct_template_taxonomies:
    - 'a:2:{s:5:"names";a:0:{}s:6:"values";a:0:{}}'
ct_use_template_taxonomies:
    - ''
ct_template_post_of_parents:
    - 'a:0:{}'
ct_template_apply_if_post_of_parents:
    - ''
ct_template_order:
    - '0'
ct_builder_shortcodes:
    - ''
oxygen_lock_post_edit_mode:
    - null
---

<figure class="wp-block-image size-large">![screenshot 2022 03 10 at 20.41.15](https://docs.dplugins.com/wp-content/uploads/2022/03/Screenshot-2022-03-10-at-20.41.15-800x615.png)</figure>The difference between Static and Variable fonts is that Variable fonts contain all font faces in one file.

## Font weight

Define font-weight ratio. On Google's Font website you can see the list with Min and Max values

<figure class="wp-block-image size-large is-resized">![screenshot 2022 03 10 at 20.44.18](https://docs.dplugins.com/wp-content/uploads/2022/03/Screenshot-2022-03-10-at-20.44.18-800x518.png)</figure>## Upload Woff and Woff2

1. You can paste CDN
2. You can paste the local path
3. You can press the upload icon and the media library will pop up. After that, you can upload font files same as any other media

## Font Display

`auto` - The font-display strategy is defined by the user agent.

`block` - Gives the font face a short block period and an infinite swap period.

`swap` - Gives the font face an extremely small block period and an infinite swap period.

`fallback` - Gives the font face an extremely small block period and a short swap period.

`optional` - Gives the font face an extremely small block period and no swap period.

## Font Italic

If activated defines that font face is italic

## Preload

It will preload web fonts using `rel="preload"` to remove any flash of unstyled text.