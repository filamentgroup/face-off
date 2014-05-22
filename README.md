# Retired

[![Filament Group](http://filamentgroup.com/images/fg-logo-positive-sm-crop.png) ](http://www.filamentgroup.com/)

This repository is now officially retired and currently resides in Florida spending its time watching daytime television and playing golf.

The code from the repo was officially merged into [Modernizr as part of Issue 1120](https://github.com/Modernizr/Modernizr/issues/1120).

---

We’re at something of a disadvantage when testing for @font-face support, as a number of platforms falsely report supporting @font-face rules, or only do so on a technicality—Windows Phone 7–7.8, for example, does only supports @font-face for fonts already installed on the device (rendering its @font-face implementation useless, but capable of passing feature tests). To work around this, we’ve blacklisted a few problematic platforms and browsers with known false positives: Android 2.1, WebOS, and Windows Phones prior to 8.

The styles that corresponding with the feature test are similar to the default styles served by Icomoon, but containing PNG fallbacks. To avoid requesting the fallback PNGs browsers that do support `@font-face`, the test has to be run prior to parsing the body of the page—specifically, prior to the browsing parsing the icon elements themselves.
