### Network Information API

(Make your website network-responsive!)

@ul
- This API lets you retrieve the current network type and monitor for network type changes.
@ulend

---

### Demo

Write connection-aware components, rendering different elements for different speeds. For example, a <Media /> component in a news article might output:
@ul
- offline: a placeholder with alt text
- 2g / reduced data mode: a low-resolution image, ~30kb
- 3g: a high resolution retina image, ~200kb
- 4g: a HD video ~1.8MB
@ulend

---

### Demo (Continued)

![Demo of Network Information API](template/img/network-information-demo.jpg)

---

### Use Cases

@ul
- Connection-aware components
- Cellular / Wifi
- Metered connection
@ulend

Note:
- Use service workers to return hi-res or lo-res images depending on the connection.
- Determine whether to preload resource-intensive assets, such as video, based on network connection (deciding to not preload assets if they're over cellular).
- Conditionally load images, videos, fonts and other resources based on whether the user is on a metered connection (such as pay-as-you-go) and his bandwidth.
