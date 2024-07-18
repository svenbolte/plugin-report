=== Plugin Report ===
Contributors: roytanck, zodiac1978, pedromendonca, PBMod
Tags: admin, plugins, multisite, report
License: GPLv3
Version: 9.2.1.1.22
Stable tag: 9.2.1.1.22
Requires at least: 6.0
Tested up to: 6.6
Requires PHP: 8.2

A WordPress plugin that provides detailed information about currently installed plugins.

##Plugin Report will allow you to:

* Spot plugins that are no longer maintained.
* Get a quick overview of the "plugin health" of your site.
* Provide clients with a detailed report, right from their own dashboard, or as CSV spreadsheet.
* Find plugins that are no longer active on multisite installs

== Screenshots ==
1. Your plugin report is found under the Plugins menu, or in the Network section if your site is a multisite install.

== Credits ==
Special thanks go to [Tristen Forsythe Brown](http://tristen.ca/) for the [tablesort JavaScript library](https://github.com/tristen/tablesort) licensed under the MIT License.

== Changelog ==

= 9.2.1-10 (2022-05-25) =
from master: Added detection for plugins that have been closed in the wordpress.org repository
changed listing, if not on wordpress but on github repository or forked, forked and closed dont get critical color unless still updated

= 9.2.0.2.8-10 (2022-05-25) =
more information about used theme and compatibility
csv export line break fixing

= 9.2.0.2.7 (2022-02-18) =
Tablesort updates
fixed some php warnings
changes from master pulled

= 9.2.0.1.7 (2022-02-03) =
from master: fixed warnings of missing variable declaration
wp 5.9 compatibility

= 9.2.0.0.7 (2021-12-17) =
pulled from master:
* Added a new column to display repository information and detect possible supply chain issues
* Tablesort updated to the latest version

= 9.1.9.3.7 (2021-12-12) =
pulled from master branch:
* Fixed an issue where the exported CSV filename contained the wrong month (thanks, @zodiac1978)
* Skip the wordpress.org API call if the plugin's Update URI is set (thanks, @zodiac1978)
* Tested with WP 5.8.2

= 9.1.9.1.7 (2021-05-02) =
* Fixed a minor issues that could cause problems with the plugin's translations.

= 9.1.9.0.7 (2021-05-02) =
* Display translated plugin info when available (thanks, @zodiac1978)
* Fixed default sorting of plugins to match WP's plugins screen (thanks, @zodiac1978).

= 9.1.8.3.7 (2021-03-21) =
from master branch: Fixed an issue where plugin auto-updates were not displayed correctly

= 9.1.8.2.7 (2021-03-09) =
percentage value fix on rating column

= 9.1.8.2.6 (2020-10-20) =
get translated description of plugins, if available
take javascript sources from the master branch
apply changes to the code

= 9.1.8.4 (2020-10-20) =
More detailed Data from local readme or plugin header - plugins without wordpress repository will be documented in list:
  * TestedUpTo, MinPHP Version, Min Wordpress Version
  * Plugin Description added in author column, some line breaks for formatting
  * all list content will be shown without line breaks in csv export in excel

= 9.1.8.3 (2020-08-17) =
display Wordpress-Plugin-Site-Link if present
count installed plugins and display at title
css fixed removed static table column layout. 
german and german formal translations updated and set to local ocation under languages in plugin folder

= 9.1.8 (2020-08-17) =
* Fixed a jQuery issue causing errors in WP 5.5
* Added column to display whether a plugin is set to auto-update

= 9.1.7 (2020-08.15)
* Add column with direct edit link, file created, file modified
* display tested up to and min php version read from local plugin (for those not having a wordpress site or being disabled on wp site

= ^^ FORKED with contribution to the master project =

= 1.7 (2020-04-03) =
* Adds column sorting (props @zodiac1978)
* Replaces the Excel export with a more robust CSV export function
* Uses HTML's progress element for the progress bar

= 1.6.1 (2020-03-21) =
* Fixed an issue with version comparisons and beta/RC versions (thanks @zodiac1978)
* Coding standards improvements (thanks @zodiac1978)
* The plugin can now only be network-activated on multisite
* Tested against WordPress 5.4

= 1.6 (2020-03-14) =
* Further i18n improvements (thanks @pedromendonca)
* Minor version differences no longer shown as "medium" risk
* When a plugin upgrade requires platform upgrades, this is now shown (suggested by @zodiac1978)
* Improved the way CSS and javascript files are enqueued

= 1.5 (2020-02-09) =
* The activation column now shows the number of activations on multisite
* I18n improvements (thanks @pedromendonca!)

= 1.4 (2020-01-17) =
* Adds an .xls export function (experimental)
* Adds an "activated" column to the report table

= 1.3 (2019-11-29) =
* Better table styles, inluding call background colors
* Improved error messages
* Cached information is now automatically refreshed when a plugin is updated through wp-admin

= 1.2 (2019-11-26) =
* Removed the "compatibility" column (data no longer provided by API)
* Fixed an issue with long plugin slugs causing invalide transient keys
* Fixed an issue where version number colors were inconsistent

= 1.1 (2019-11-23) =
* Code cleanup
* Adds proper multisite support
* Accessibility and internationalisation improvements
 
= 1.0 (2017-01-17) =
* Initial version