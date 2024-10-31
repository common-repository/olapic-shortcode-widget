=== Olapic Shortcode Plugin ===
Contributors: olapic
Tags: olapic
Requires at least: 3.7
Tested up to: 5.5
Stable tag: 3.3.4
License: GPLv2 or later

A shortcode plugin allowing users to use shortcodes to surface Olapic Javascript codes on WordPress posts

== Description ==

The #1 Visual Commerce & Marketing Platform. Olapic turns consumer-generated content into your most valuable brand asset.

What we believe: White backdrops, studio lighting, and simulated friend groups don’t get people’s attention anymore. Nor do they drive sales like they once did. Brands need better content that relates to their audiences’ lives, and they need more of it to fill the growing number of relevant channels while driving towards their business goals.

This plugin allows users to utilize shortcodes to embed Olapic Javascript widgets on WordPress posts.

== Installation ==

Using this plugin involves a simple three-step process:

1. Upload the plugin files to the `/wp-content/plugins/plugin-name` directory, or install the plugin through the WordPress plugins screen directly.

2. Activate the plugin through the 'Plugins' screen in WordPress

3. In the Wordpress post, use the Olapic shortcode as follows: 

    `[olapic instance-id="WIDGET_INSTANCE_ID" apikey="OLAPIC_API_KEY" tags="PRODUCT_ID lang="LANG_CODE" - if applicable"]`. 

Voila! You're set!

**Shortcode Attributes:**

* `instance-id` - **required**
    * You can find this value from the `data-instance` part of the original widget code.
* `apikey` - **required**
    * You can find this value from the `data-apikey` part of the original widget code. 
* `tags` - *optional*
    * This serves as the dynamic identifier to pull content from a specific stream. Often, the value is the product identifier from your product feed.
* `lang` - *optional*
    * The language code that you want the widget to be translated to. The naming convention for the language's name is based on the ISO-639 language code (e.g. pt for Portuguese) followed by the ISO-3166 country code (e.g. _PT for Portugal or _BR for Brazil), and corresponds with the language codes set in the "appearance" section of the Olapic platform.
* `mode` - *optional*
    * Accepted parameter value: `development`
    * You can use this flag to serve all content from the sandbox environment.
    * Note that this parameter ***should not*** be utilized for production purposes.
