# Flarum PWA

Turns Flarum into a basic progressive web app. If a user loses connection, an offline page will appear with a simple message alerting them that this app does not work offline. As of version 1.1, this PWA no longer attempts to cache pages. This is because it was discovered that, in certain browsers / on certain devices, the extra caching was causing users to have to manually refresh pages in order to complete tasks such as logging out or logging in. However, even without caching this is useful because it gives users another option: the ability to install your forum and open it in a standalone app window.

This is what you see and to install in Chrome (on a desktop). Each browser and device will handle this differently.
![](https://i.ibb.co/H4PBm8p/Screenshot-2019-09-28-at-5-27-26-AM.png)

Here is the experience after it is installed on a Chromebook:
https://vimeo.com/362968169

## Install instructions

#### Pre-install:

1. **Required:** Add [sw.js](https://github.com/zerosonesfun/pwa/blob/master/assets/sw.js) to the public root of your site (i.e. /public_html/, /home/, or whatever your public root is called).
2. **Required:** Add [site.webmanifest](https://github.com/zerosonesfun/pwa/blob/master/assets/site.webmanifest) to the public root of your site (/public_html/, /home/, or whatever your public root is called).
3. _Optional:_ Edit the site.webmanifest file. Change the name of the app, where the app icons are located, and even the theme color and background color settings. **Do not** change the start url or scope unless you know what you're doing.

#### Install:

4. `composer require zerosonesfun/pwa`

#### Update:

`composer update zerosonesfun/pwa`

#### Links:
- Github: [https://github.com/zerosonesfun/pwa](https://github.com/zerosonesfun/pwa)
- Packagist: [https://packagist.org/packages/zerosonesfun/pwa](https://packagist.org/packages/zerosonesfun/pwa)
- Me: [https://wilcosky.com](https://wilcosky.com)
