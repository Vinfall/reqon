# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [3.5.4] - May. 7, 2024
- Bump dependencies.

## [3.5.3] - Apr. 8, 2024
- Update Spanish translation.

## [3.5.2] - Apr. 7, 2024
- Squash on latest submodule version.
- Fix eslint error.

## [3.4.1] - Apr. 6, 2024
- Rename to reqon.
- Fix jest test error.

## [3.3.0] - Apr. 2, 2024
- Update dependencies.

## [2.0.0] - Apr. 2, 2024
- Introduce numerous fixes & new bugs.

## [1.16.0a1] - Dec. 24, 2021
- Add option to remove toolbar icon counter. #129
- Add support for matching hostnames without suffix (TLD wildcard). #126
- Add private browsing matcher to ignore or only use in private browsing.

## [1.15.5] - Jul. 7, 2020
- Fix rule creation after 1.15.3. #131

## [1.15.4] - Jul. 3, 2020
- Fix required validation after 1.15.3. #131

## [1.15.3] - Jul. 3, 2020
- Fix Redirect rule not being applied when multiple rules were matching a single request. #111
- Fix rule tester with multiple redirect rules.
- Remove backspace deleting added parameters. #128

## [1.15.2] - Mar. 28, 2020
- Fix Filter rule not being applied when multiple filter rules were matching a single request. #111

## [1.15.1] - Mar. 13, 2020
- Fix popup height when placed to overflow menu. #111
- Fix rule tester regexp escaping. #113
- Fix selected rules exporting.

## [1.15.0] - Mar. 11, 2020
- Add Secure action to upgrade HTTP requests to HTTPS.
- Add new default rules: FBCLID stripping rule and FB redirection service rule. #110 by @AreYouLoco
- Fix text color when default color is changed. #112 by @Zocker1999NET
- Fix filter/redirect actions to be applied and logged separately.
- Remove Downloads API dependency for rule export.
- Update icons and badge color.

## [1.14.0] - Sep 8, 2019
- Add option to redirect document (update tab) from other requests types. #103
- Fix invalid regexp pattern breaking all other rules. #107
- Keep last record when redirect/filter rule is followed by a server redirection.

## [1.13.3] - Aug 22, 2019
- Fix hosts/paths input field overflow issue with long list of values (2nd fix). #104
- Fix updating of input fields for merged rules after import.
- Accept text files on import.

## [1.13.2] - Aug 19, 2019
- Fix comma not accepeted in includes/excludes input fields. #105
- Fix hosts/paths input field overflow issue with long list of values. #104

## [1.13.1] - Aug 10, 2019
- Fix subdocument redirect regression issue #103
- Fix bad localization key.

## [1.13.0] - Aug 5, 2019
- Change query parameter trimming in Filter Rule to not apply to the extracted redirect URL. #99
- Add replace all substring support for Redirect Rule. #101

## [1.12.4] - June 29, 2019
- Add workaround for Firefox bug https://bugzilla.mozilla.org/show_bug.cgi?id=1557300. #100
- Other improvements to options (rule delete button, create button / new rule validation fix, type badge)

## [1.12.3] - May 12, 2019
- Update style and manual.
- Fix rule edit link in popup.

## [1.12.2] - April 28, 2019
- Order rules alphabetically. #90

## [1.12.1] - April 27, 2019
- Update style for more compact layout.

## [1.12.0] - April 22, 2019
- Add Android support and update layout and style for mobile browsers. #88
- Add speculative request type. #81
- Add support for matching requests by origin. #36
- Close modals on Escape-key. #91
- Fix action buttons disabled issue. #96
- Fix white list rule testing no feedback issue. #92
- Fix percent sign issue with redirect rules. #95

## [1.11.1] - September 6, 2018
- Add strict min version requirement for Firefox 60.
- Remove debug console logging #80.

## [1.11.0] - August 17, 2018
- Add support for skipping redirection url filtering within same domain. #29

## [1.10.1] - August 4, 2018
- Fix excludes/includes with Any URL. #77

## [1.10.0] - July 29, 2018
- Add keywords to decode and encode captured patterns for redirect rule #6
- Add includes and excludes pattern support #16 #24 #35
- Add option to control whitelist logging #59
- Add query parameter expansion support for redirect rule #72
- Change to trim unwanted query parameters before inline url parsing #72
- Update active and disabled icons #70
- Fix parsing of redirect instructions with inline brackets #73

## [1.9.4] - May 26, 2018
- Fix rule import after 1.9.3 changes.
- Fix showing number of selected rules for new rules.

## [1.9.3] - May 24, 2018
- Add alphabetizing patterns. #57
- Add Select / select none input #63
- Add showing number of selected rules #64
- Add UUID for rules. Rules with same UUID will be overwritten when importing rules.
- Fix Rule Tester to escape '?' in path. #65
- Fix redirecting by manipulating 'hostname'. #69

## [1.9.2] - May 15, 2018
- Add disabled state icon.
- Fix resolving match patterns with multiple paths and TLDs. #66

## [1.9.1] - May 13, 2018
- Fix toolbar icon updating.
- Fix adding two-character long generic domains. #56
- Fix adding comma to trim parameters. #58

## [1.9.0] - May 9, 2018
- Add rule tester for testing selected rules against test URL.
- Add support for rule tagging in panel.
- Add rule edit links in panel.
- Add disable/enable button in panel.
- Change Redirect instructions to supports parameter expansion in value.
- Update options style and panel layout.
- Locale: ES Spanish, thanks to @strel at Github!

## [1.8.6] - Nov. 26, 2017
- Fix Redirect to static url.
- Fix combining parameter expansion with redirect instructions.
- Add unit tests.

## [1.8.5] - Nov. 25, 2017
- Fix query parameter trimming. #50
- Fix icons not showing in rules view.

## [1.8.4] - Nov. 18, 2017
- Fix build.

## [1.8.3] - Nov. 17, 2017
- Fix regex repetition quantifier not supported in pattern captures. #45 #47
- Fix query parameters trimming on non-standard urls. #48 #40

## [1.8.2] - August 6, 2017
- Fix Filter rule to always decode redirection URL.
- Add version in about page.

## [1.8.1] - July 22, 2017
- Fix save rule on title/description change.
- Fix any-url host input required validation.
- Add description for default rules.
- Load default rules from file ("/options/default-rules.json").
- Strip paramsTrim pattern from exported rules.

## [1.8.0] - July 19, 2017
- Rules are now auto saved on change.
- Rule name and description are editable.
- Add invert URL parameter trim option.
- Add about page.
- Other changes to rule options display.

## [1.7.1] - July 1, 2017
- Fix whitelist/block rule request markers.
- Fix migrate script for Firefox versions before 55.

## [1.7.0] - June 29, 2017
- Add rules export and import. #8
- Add toolbar button to list details of applied rules on current tab. #19
- Add tabs to options view.
- Fix trim parameter inconsistency: support literal string params and regexp params. #17
- Fix pageAction details bug with block rules. #19
- Fix filter rule redirection url filtering. #20
- Remove url status icon. #19

## [1.6.1] - June 21, 2017
- Add i18n support
- Add request details in page action popup
- Fix query parameters trim with valueless params

## [1.6.0] - June 13, 2017
- Add support for multiple rule matching for single request.
- Add support for adding multiple hosts and paths for rules.
- Remove 'Include subdomains' checkbox.
- Improve rules options view.

## [1.5.0] - June 1, 2017
- URL parameter filtering is now Filter rule specific.
- Redirection cleaning can now be turned off in Filter rule.
- Added wildcard "*" support for url parameter trimming.

## [1.4.3] - May 27, 2017
- Fix url parameter filtering for global rules.
- Fix redirection url parsing from query string.
- Fix default google filter rule, include main frame requests.
- Fix filter action handler to only do tab navigation on sub_frame requests.

## [1.4.2] - May 7, 2017
- Fix to escape forward slash in replace regex pattern.
- Add toggle rule edit on double click.

## [1.4.1] - April 12, 2017
- Change the default type for new rules to be the document type.
- Change any url and any type buttons to be the rightmost on rule panel.
- Fix more than one parameter expansions failing in redirection address.
- Fix undefined rule title when saving a new rule without changing its action.

## [1.4.0] - April 10, 2017
- Add support for pattern capturing (parameter expansion) to redirect based on the original request.
- Add support for parameter instructions to redirect based on the original request.
- Change help page to open in a new page.
- Update help and add attributions to the MDN documents.
- Fix missing title for options page.

## [1.3.0] - March 27, 2017
- Add whitelist rules support.
- Add <all_urls> pattern support for creating global rules.
- Change option page to open in new tab.
- Fix input validation that allowed incorrect rule saving.

## [1.2.3] - March 15, 2017
- Add toggleable edit mode for rules.
- Change tracking URL parameters input option to use one line tags-input.
- Fix to include WebExtension permission for all urls.
- Fix to include applications key with add-on id in manifest.json.

## [1.2.2] - October 30, 2016
- Add support for rule based control with actions (filter, block, redirect).
- Add support for request types.
- Add page action for providing user feedback of handled requests.
- Add help page.
- Add "ng" to the TLDs of pre-defined rule for Google.
- Fix subdomain top-level domain confusion.
- Change TLDs from global list to rule based manual list.
- Change add-on name from JustRedirect! to Request Control.
- Change license from MIT to MPL-2.0.
- Enhance options usability to improve rule creation and match pattern definition (uses Bootstrap CSS).

## [1.1.0] - October 1, 2016
- Add match pattern for Google search to prevent outgoing search link tracking.
- Add support for creating match patterns for matching different sub domains (e.g. www.google.*).
- Add match pattern validation.
- Add icon for the add-on.
- Fix to prevent enter key from deleting values on inputs.
- Fix updating redirection listeners on options change.
- Fix adding history entries for redirection origin urls.

## [1.0.2] - September 24, 2016
- Add out.reddit.com redirection url pattern.
- Add outgoing.prod.mozaws.net pattern.
- Fix query parameter filtering.

## [1.0] - September 23, 2016
- Initial release
