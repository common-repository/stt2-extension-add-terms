=== STT2 Extension Add Terms ===
Contributors: Jevuska
Donate link: https://www.jevuska.com/donate/
Tags: post, searchterms, keywords, seo, tagging, search, stt2, postmeta, shortcode, widget, term
Requires at least: 4.4
Tested up to: 4.7
Stable tag: 1.2.3
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Add your terms into single post manually, get terms via referrer, and save them as post meta.

== Description ==
Manage your terms better, add terms into single post manually, get terms via referrer, and save them as post meta. Search the terms that relevant of post content as well as WordPress search default algorithm.

= Features =
 * Save terms as postmeta ( private meta_key ).
 * Manual input terms into postmeta.
 * Get terms via referrer ( ajax or PHP ).
 * Better terms characters input.
 * Characters length of terms is min 4 and max 70.
 * Show terms list in front end ( ajax or html ).
 * General settings, multiple widgets, and shortcode `[stt2extat]`.
 * Terms stats.
 * Manual or scheduling to delete unused terms.
 * Convert text of terms into link ( post or search link ).
 * Easy setup search link structure under options permalink page.
 * Hook `wp_head` on search page to include canonical rel, and add meta no robots if no posts found.
 * Set 404 page by hook `pre_get_posts` on search page if term is not allowed or empty ( as note, Headers status code is 200, not 404 ).
 * More features and filters available ( see: [ Plugin page ](https://www.jevuska.com/2015/06/28/injeksi-manual-keyword-add-onsextension-plugin-seo-searchterms-tagging-2/ "Plugin page") ).
 
= Requirement =
 * jQuery latest version
 * WordPress min version 4.4
 * PHP Server min version 7.0
 
= Package =
 * The excerpt preview of terms result is supported by Plugin Search Excerpt by Scott Yang
 * Autocomplete terms suggestion is supported by Google Suggest for jQuery plugin by Haochi Chen

= Next Feature =
 * Convert terms into custom taxonomy and feature on terms meta
 
== Installation ==
1. Upload the entire `STT2 Extension Add Terms` folder to the `/wp-content/plugins/` directory.
2. Activate the plugin through the `Plugins` menu in WordPress.
3. Configure your `STT2EXTAT` settings and you are ready to go.
4. Multiple Widget available under title `STT2EXTAT Terms List`
5. You can use shortcode `[stt2extat]` to show terms list inside post content.

== Frequently Asked Questions ==
= My server not support for PHP 7, may I use this plugin? =
You can use *Undevelopment version* of this plugin. Please checkout the [Developers](https://wordpress.org/plugins/stt2-extension-add-terms/developers/ "Developers") page and use `1.1.5-undev` version. It's the same features with `v1.1.5`.

= Can I add bulk terms ? =
Yes, you can. After you add one or more terms via input field, just add your terms list that separated by comma or add per-line into textarea.

== Screenshots ==
1. STT2EXTAT General Settings
2. STT2EXTAT Manual Insert Tool and Term Stats
3. STT2EXTAT Multiple Widget
4. STT2EXTAT Permalink for search page

== Changelog ==
* 1.2.3 = December 27, 2016
 * Fixes jquery-stt2extat.js admin, and function stt2extat_parse_url
 
* 1.2.2 = July 01, 2016
 * Fixes posts_per_page post without terms
 
* 1.2.1 = April 23, 2016
 * Fixes bug for user caps and search excerpt
 
* 1.2.0 = April 09, 2016
 * Fixes terms list count.
 
* 1.1.9 = December 22, 2015
 * Fixes search excerpt.
 
* 1.1.8 = December 21, 2015
 * Fixes update notice.
 * Patch function exist for `array_column`.
 
* 1.1.7 = December 21, 2015
 * Fixes plugin setup

* 1.1.6 = December 20, 2015
 * Fixes readme files.
 * Identified array or object with `array_column` only.
 * Remove `stt2extat_filter_search_page_title`.
 * Add function `stt2extat_search_page_title` to filter `document_title_parts`, in comment, see hook.php.
 * Add function `stt2extat_search_page_title_separator` to filter `document_title_separator`, in comment.
 * Change a function's name `stt2extat_get_relevant_post_on_search_page` into `stt2extat_get_the_id_relevant_post`.
 * Fixes `lib/content/templates` files.
 * Fixes screen option.
 * Fixes hook.
 * Fixes translation.
 
* 1.1.5 = December 17, 2015
 * Fixes parse_request and patch `set_404` as `pre_get_posts` for not allowed terms on search page.
 * Normalize path
 * Fixes list on textarea
 * Add `per_page` number on Screen Options and search box for Term Stats table
 * Fixes ajax tabel pagination
 * Fixes translation bahasa Indonesia
 * Fixes readme files
 * Delete `content-create-tax.php` file, its not ready to setup yet
 
* 1.1.4 = December 16, 2015
 * Fixes wp_get_referer
 
* 1.1.3 = December 16, 2015
 * Fixes bug on search excerpt plugin
 
* 1.1.2 = December 16, 2015
 * Fixes bug empty array when scheduling to delete unused terms
 
* 1.1.1 = December 16, 2015
 * Patch `wp_list_pluck` when `array_column` function undefined during installation, even this plugin no longer support server with PHP versions lower than 7.
 * Fix `jquery-stt2extat.js` to enable `enter` key when input terms into textarea.
 
* 1.1.0 = December 15, 2015
 * Create admin plugin
 * Available to get terms via referrer
 * Insert terms as post meta
 * Shortcode and widget available
 * Sanitizing input and output of incoming terms
 * Add Search Excerpt plugin for search page snippet
 * Fix hook setup on activation an deactivation
 * Delete files stt2extat-x.x.x.php (x.x.x = version), and create stt2extat-1.1.0.php include in stable minor version 1.1
 * Add comments in each functions
 * Fix translation in Bahasa Indonesia
 * WordPress version 4.4
 * PHP Server version 7.0
 
* 1.0.4 = October 26, 2015
 * Change short syntax for arrays at `stt2extat_insert_callback` to work under PHP 5.4
 
* 1.0.3 = October 25, 2015
 * Sanitize, escape, and validate POST, REQUEST calls
 * Remove old jquery UI, use jQuery UI WP Core
 * Update jquery-stt2extat.js
 * Remove unused files and fixes other functions for a security related bug

* 1.0.2 = October 16, 2015
 * Fix readability code
 * Fix undefined variable
 * Internationalize plugin
 * minify version jquery-stt2extat.min.js
  
* 1.0.1 = October 13, 2015
 * Remove session PHP
 * Add update plugin check
 * Add Screenshoot

* 1.0.0 = June 28, 2015
 * First official release!

== Upgrade Notice ==
= v1.2.3 =
Fixes jquery-stt2extat.js admin, and function stt2extat_parse_url. Upgrade immediately.

= v1.2.2 =
Fixes posts per page without term in admin panel. Upgrade immediately.

= v1.2.1 =
Fixes search excerpt related bug. Upgrade immediately.

= v1.2.0 =
Fixes terms count related bug. Upgrade immediately.

= v1.1.9 =
Fixes search excerpt related bug. Upgrade immediately.

= v1.1.7 =
Fixes setup bug. Upgrade immediately.

= v1.1.6 =
Fixes manual input templates and improvement searching data. Please upgrade yours.

= v1.1.5 =
Fixes not found search result and bug ajax pagination. Please upgrade yours.

= v1.1.4 =
Fixes referrer. Upgrade immediately.

= v1.1.3 =
Fixes a security related bug. Upgrade immediately.

= v1.1.2 =
Fixes error on scheduling delete unused terms.

= v1.1.1 =
Fixes error during installation with PHP versions lower than 7.

= v1.1.0 =
This new minor and patch version to fixes a security related bug. Upgrade immediately.

= v1.0.3 =
This version fixes a security related bug.  Upgrade immediately.

= v1.0.2 =
This version fixes a security related bug.  Upgrade immediately.

== Note ==
Search Excerpt plugin under package of this plugin, a setting available to enable or disable it.