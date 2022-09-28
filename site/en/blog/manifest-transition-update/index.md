---
layout: 'layouts/blog-post.njk'
title: More details on the transition to Manifest V3
description: >
  Details of the gradual approach to phasing out of Manifest V2 extensions.
subhead: >
  Details of the gradual approach to phasing out of Manifest V2 extensions.
date: 2022-09-28
authors:
  - dsli
tags:
  - extensions
hero: image/kheDArv5csY6rvQUJDbWRscckLr1/PRhcGmihtca0AyHkfLcs.jpg
alt: A sunset.
---

Last year, we [announced](/blog/mv2-transition/) a timeline for the phasing out of Manifest V2 extensions as we shift our focus to Manifest V3. This change will give Chrome users increased safety and peace of mind while browsing and installing extensions by providing more transparency and control over permissions, adding stricter protocols for accessing resources outside the extension's context, and ensuring that extensions work well on all devices.

Chrome will take a gradual and experimental approach to turning off Manifest V2 to ensure a smooth end-user experience during the phase-out process. We would like to make sure developers have the information they need, with plenty of time to transition to the new manifest version and to roll out changes to their users.  In support of that goal, we're providing more details about how Chrome will phase out Manifest V2 support. 

Specifically:

-  Starting in January on **Chrome 112**, Chrome may run experiments to turn off support for Manifest V2 extensions in Canary, Dev, and Beta channels.
-  Starting in June on **Chrome 115**, Chrome may run experiments to turn off support for Manifest V2 extensions in all channels, including Stable channel.

For developers who still own extensions running Manifest V2, we recommend completing migration to Manifest V3 well ahead of the release of these Chrome versions because those extensions may stop working at any time following the aforementioned dates.

For enterprises, we are extending Manifest V2 support via [the ExtensionManifestV2Availability enterprise policy](https://bugs.chromium.org/p/chromium/issues/detail?id=1347794) to January 2024. Additional details may be found on our [Manifest V2 support timeline page](https://developer.chrome.com/docs/extensions/mv3/mv2-sunset/).

We also have a few updates on how the phase-out will look on the Chrome Web Store:

-  In **January 2023**, use of Manifest V3 will become a prerequisite for the [Featured badge](https://blog.google/products/chrome/find-great-extensions-new-chrome-web-store-badges/) as we raise the security bar for extensions we highlight in the store.
-  In **June 2023**, the Chrome Web Store will no longer allow Manifest V2 items to be published with [visibility](https://developer.chrome.com/docs/webstore/cws-dashboard-distribution/#setting-the-visibility) set to Public. All existing Manifest V2 items with visibility set to Public at that time will have their visibility changed to Unlisted.
-  In **January 2024**, following the expiry of the Manifest V2 enterprise policy, the Chrome Web Store will remove all remaining Manifest V2 items from the store.

In addition, we have been working with extension developers to improve Manifest V3 and to incorporate feedback from our community. Based on developer feedback, in recent months we've supplemented service worker functionality, introduced new APIs, and made a number of other platform improvements. 

We know that some members of our community are paying close attention to in-progress feature additions and bug fixes to the Manifest V3 platform. To provide greater transparency to our community, we are also adding a [progress page](https://docs.google.com/document/u/0/d/1s59_ALwSOL1djxZz7G0l6PjZcXBM3SR9Cjejuwo5BlM/edit?resourcekey=0-kljyHBOJ_eKYsaQs1XLBiw) for interested developers to keep track of top priority issues Chrome is tackling before the turn-down experiments.

We thank all of our developers who have provided valuable feedback over the past year as they've migrated their extensions to Manifest V3. We're excited to see the growth of adoption from developers who are creating new extensions and migrating existing ones. We also want to thank the many developers in our community who have stepped up to provide guidance to others with similar questions. If you have feedback or comments, please continue to let us know by posting to the [chromium-extensions](https://groups.google.com/a/chromium.org/g/chromium-extensions) Google Group.

We look forward to continuing to work together to make the extension ecosystem vibrant, performant, and trustworthy.

_Photo by [David Mullins](https://unsplash.com/@mullins?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)_