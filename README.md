[![BuildStatus](https://github.com/tumpio/requestcontrol/workflows/Build/badge.svg?event=push&branch=master)](https://github.com/tumpio/requestcontrol/actions)

# Request Control - Firefox extension

An extension to control HTTP requests. Provides front-end for Firefox
[webRequest.onBeforeRequest](https://developer.mozilla.org/en-US/Add-ons/WebExtensions/API/webRequest/onBeforeRequest)
API for HTTP request management.

Requests can be controlled with following rules:
- Filter Rule: Skip URL redirection and remove URL query parameters.
- Redirect Rule: Rewrite requests with support for [Pattern Capturing](https://github.com/tumpio/requestcontrol/blob/master/_locales/en/manual.wiki#redirect-using-pattern-capturing) to redirect based on the original request.
- Secure Rule: Upgrade non-secure (HTTP) requests to secure (HTTPS).
- Block Rule: Block requests before they are made.
- Whitelist Rule: Whitelist requests from other rules.

Other useful information:
- [Manual](https://github.com/tumpio/requestcontrol/blob/master/_locales/en/manual.wiki)
- [FAQ](https://github.com/tumpio/requestcontrol/issues?utf8=%E2%9C%93&q=label%3Aquestion+)
- [Source code](https://github.com/tumpio/requestcontrol)
- [License](./LICENSE)

## Support

- Report bugs
- Suggest new features
- Help to translate
- Contribute

## Development

Clone repository and setup development environment with npm:

```sh
git clone https://github.com/tumpio/requestcontrol.git
cd requestcontrol
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
```

## External Libraries

Request Control uses the following external libraries:

- [lit](https://ajusa.github.io/lit/) is licensed under the MIT license.
- [tags-input](https://github.com/developit/tags-input) and its fork by [\@pirxpilot](https://github.com/pirxpilot/tags-input) are licensed under the MIT license.
- [ionicons](http://ionicons.com/) is licensed under the MIT license.
- [tldts](https://github.com/remusao/tldts) is licensed under the MIT license.

## [License](./LICENSE)

    This Source Code Form is subject to the terms of the Mozilla Public
    License, v. 2.0. If a copy of the MPL was not distributed with this
    file, You can obtain one at http://mozilla.org/MPL/2.0/.
