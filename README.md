[![BuildStatus](https://github.com/Vinfall/reqon/actions/workflows/build.yml/badge.svg?event=push&branch=master)](https://github.com/Vinfall/reqon/actions)

# Reqon (fork of *[Request Control](https://github.com/tumpio/requestcontrol)*)

An extension to control HTTP requests. Provides front-end for Firefox
[webRequest.onBeforeRequest](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/API/webRequest/onBeforeRequest)
API for HTTP request management.

Requests can be controlled with following rules:
- Filter Rule: Skip URL redirection and remove URL query parameters.
- Redirect Rule: Rewrite requests with support for [Pattern Capturing](https://github.com/Vinfall/reqon/blob/master/_locales/en/manual.wiki#redirect-using-pattern-capturing) to redirect based on the original request.
- Secure Rule: Upgrade non-secure (HTTP) requests to secure (HTTPS).
- Block Rule: Block requests before they are made.
- Whitelist Rule: Whitelist requests from other rules.

Other useful information:
- [Manual](https://github.com/Vinfall/reqon/blob/master/_locales/en/manual.wiki)
- [Community-maintained ruleset](https://github.com/Vinfall/reqon-rules)
- [Source code](https://github.com/Vinfall/reqon)
- [License](./LICENSE)

## Installation

1. Open `about:addons`
2. Click on the gear icon (⚙️)
3. Click `Install Add-on From File...`
4. Select the zip you downloaded from [releases](https://github.com/Vinfall/reqon/releases/latest)
5. Now you are good to go! Open options to check if rules are kept and test the functionality

## Support

- Bug Report
- Feature Suggestion
- Localization
- Code Contribution
- Rule Contribution

## Development

Clone repository and setup development environment with npm:

```sh
git clone https://github.com/Vinfall/reqon.git
cd reqon
npm i
```

Run in Firefox-nightly:

```sh
npm start -- --firefox=nightly
```

Run unit tests and lint:

```sh
npm test
npm run lint
```

Build extension:

```sh
npm run build
npm run lint-build
```

## External Libraries

Reqon uses the following external libraries:

- [lit](https://ajusa.github.io/lit/) is licensed under the MIT license.
- [tags-input](https://github.com/developit/tags-input) and its fork by [\@pirxpilot](https://github.com/pirxpilot/tags-input) are licensed under the MIT license.
- [ionicons](http://ionicons.com/) is licensed under the MIT license.
- [tldts](https://github.com/remusao/tldts) is licensed under the MIT license.

## [License](./LICENSE)

    This Source Code Form is subject to the terms of the Mozilla Public
    License, v. 2.0. If a copy of the MPL was not distributed with this
    file, You can obtain one at http://mozilla.org/MPL/2.0/.
