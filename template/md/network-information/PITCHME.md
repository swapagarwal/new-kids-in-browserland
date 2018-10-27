---?image=template/meme/is_impossible_to_read_on_my_smartphone.jpg&size=auto 100%

Note:
Responsive Web Design has revolutionized the web. A single site can adapt its layout when viewed on a range of different devices and screens. All that's required is a few media queries to detect the screen size and load alternative CSS.

However, using the screen size to detect browser capabilities is similar to judging a car's speed by looking at its radio. Modern smartphones and tablets have increasingly large resolutions and will happily show a typical desktop view. If that view adds numerous fonts, images or other assets, the mobile user may receive a degraded — and expensive — experience when they're on a slower or metered connection.

---

### Network Information API

This API lets you retrieve the current network type and monitor for network type changes.

Note:
The Network Information API provides a solution here. It indicates whether the user is on a metered connection (such as pay-as-you-go) and provides an estimate of bandwidth. Using this information, it's possible to conditionally load images, videos, fonts and other resources. At a very basic level, you could override a media query to ensure the mobile layout is retained on a limited network.

---

### Example

Write connection-aware components, rendering different elements for different speeds. For example, a <Media /> component in a news article might output:
@ul
- offline: a placeholder with alt text
- 2g / reduced data mode: a low-resolution image, ~30kb
- 3g: a high resolution retina image, ~200kb
- 4g: a HD video ~1.8MB
@ulend

Note:
- You can use service workers to return hi-res or lo-res images depending on the connection.

---?image=template/img/network-information-demo.jpg&size=auto 100%

Note:
- This is how a network-responsive component may look like for different users.

---?image=template/img/carbon/network-information-preload.png&size=90% auto

@snap[north]
@size[1.5em](Preload Assets)
@snapend

Note:
- Determine whether to preload resource-intensive assets, such as video, based on network connection (deciding to not preload assets if they're over cellular).

---?image=template/img/carbon/network-information-monitor.png&size=90% auto

@snap[north]
@size[1.5em](Monitor)
@snapend

Note:
- Conditionally load images, videos, fonts and other resources based on whether the user is on a metered connection (such as pay-as-you-go) and his bandwidth.

---?image=template/img/caniuse/network-information.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
https://caniuse.com/#feat=netinfo
@snapend

Note:
This is supported on Chrome and Firefox for Android. Support for other platforms is coming soon.
