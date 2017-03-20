
# jsonrequest

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Travis](https://img.shields.io/travis/IonicaBizau/jsonrequest.svg)](https://travis-ci.org/IonicaBizau/jsonrequest/) [![Version](https://img.shields.io/npm/v/jsonrequest.svg)](https://www.npmjs.com/package/jsonrequest) [![Downloads](https://img.shields.io/npm/dt/jsonrequest.svg)](https://www.npmjs.com/package/jsonrequest)

> A tiny library for requesting and getting JSON resources.

## :cloud: Installation

```sh
$ npm i --save jsonrequest
```


## :clipboard: Example



```js
// Dependencies
var request = require("jsonrequest");

// Make a request to GitHub API
request("https://api.github.com/users/IonicaBizau", function (err, data) {
    console.log(err || data);
});
// => {
//   "login": "IonicaBizau",
//   "id": 2864371,
//   "avatar_url": "https://avatars.githubusercontent.com/u/2864371?v=3",
//   "gravatar_id": "",
//   "url": "https://api.github.com/users/IonicaBizau",
//   "html_url": "https://github.com/IonicaBizau",
//   "followers_url": "https://api.github.com/users/IonicaBizau/followers",
//   ...
// }
```

## :memo: Documentation


### `jsonRequest(options, data, callback)`
Creates the http(s) request and parses the response.

#### Params
- **String|Object** `options`: A string representing the request url or an object passed to the `tinyreq` function.
- **Object** `data`: The request data object.
- **Function** `callback`: The callback function.

#### Return
- **Object** The request object.



## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:


## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:


 - [`bnotify`](https://github.com/IonicaBizau/bnotify)—A notification system written in NodeJS using the BAT platform.
 - [`gh.js`](https://github.com/IonicaBizau/gh.js)—Tiny GitHub API wrapper for server and client.
 - [`homebridge-domotiga`](https://github.com/Samfox2/homebridge-domotiga#readme) (by Sam Fox)—domotiga plugin for homebridge: https://github.com/nfarina/homebridge
 - [`ipinfo`](https://github.com/IonicaBizau/node-ipinfo)—An http://ipinfo.io NodeJS wrapper.
 - [`npm-user-pkgs`](https://github.com/IonicaBizau/npm-user-pkgs#readme)—Fetch the npm packages created by a specific user.

## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2014#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
