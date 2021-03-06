=== FA WP Admin Menu Icons ===
Contributors: ptrkcsk
Tags: fontawesome, icon, icons, custom
Requires at least: 4.4
Tested up to: 4.9.1
Requires PHP: 5.5
Stable tag: 2.0.1
License: GPLv3
License URI: https://www.gnu.org/licenses/gpl-3.0.en.html

Use Font Awesome icons for custom post types and custom menu pages.

== Description ==

Use Font Awesome icons for custom post types and custom menu pages.

    register_post_type( 'custom_post_type', [
        //...
        'menu_icon' => 'fas fa-thumbs-up',
        //...
    ] );

[FA WP Admin Menu Icons on GitHub](https://github.com/ptrkcsk/fa-wp-admin-menu-icons)

== Usage ==

FA WP Admin Menu Icons works for the following WordPress functions:

- `register_post_type()`
- `add_menu_page()`

**Custom post type**

    register_post_type( 'custom_post_type', [
        //...
        'menu_icon' => 'fas fa-thumbs-up',
        //...
    ] );

**Custom menu page**

    add_menu_page(
        'Custom Menu Page',
        'Custom Menu Page',
        'manage_options',
        'custom_menu_page',
        '',
        'fas fa-thumbs-up', // $icon_url
    );

== Installation ==

= Composer =

    $ composer require wpackagist-plugin/fa-wp-admin-menu-icons

= Git =

    $ cd <wp-content>/plugins
    $ git clone git@github.com:ptrkcsk/fa-wp-admin-menu-icons.git

= WordPress =

[How to install WordPress plugins.](https://codex.wordpress.org/Managing_Plugins#Installing_Plugins)

== Changelog ==

= 2.0.1 =

**Added**

- Add CC BY 4.0 attribution in `icons/README.md` to adhere to [Font Awesome license](https://fontawesome.com/license)

**Fixed**

- Fix old syntax in readme examples
- Add missing 'Usage' section to `README.txt`

= 2.0.0 =

**Added**

- Add unit tests

**Changed**

- Upgrade to Font Awesome 5 icons and class syntax
- Use PSR instead of WordPress for code style

**Deprecated**

- Deprecate use of Font Awesome 4 class syntax

= 1.0.4 =

**Changed**

- Format code

**Removed**

- Remove caveat from documentation because it no longer applies

= 1.0.3 =

**Added**

- Add more icons

= 1.0.2 =

**Fixed**

- Fix undefined index

= 1.0.1 =

**Fixed**

- Add icons to `icons/`. The directory was empty on the WordPress plugin repository.

= 1.0.0 =

== Upgrade Notice ==

= 2.0.0 =

FA WP Admin Icons v2.0.0 supports Font Awesome 5!
