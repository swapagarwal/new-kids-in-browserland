### Let's talk about memory

Note:
The range of capabilities of devices that can connect to the web is wider today than it's ever been before. The same web application that's served to a high-end desktop computer may also be served to a low-powered phone, watch, or tablet, and it can be incredibly challenging to create compelling experiences that work seamlessly on any device.


---?image=template/meme//are_widely_used_in_emerging_markets.jpg&size=auto 100%

Note:
Low memory devices devices (under 512MB, 512MB-1GB) are widely used in emerging markets.

---

### Device Memory API

This API returns the amount of device memory (RAM) on a user's machine in gigabytes.

Note:
The Device Memory API is a new web platform feature aimed at helping web developers deal with the modern device landscape. It adds a read-only property to the navigator object, navigator.deviceMemory, which returns how much RAM the device has in gigabytes, rounded down to the nearest power of two.

---?image=template/img/carbon/device-memory.png&size=90% auto

@snap[north]
@size[1.5em](Code Sample)
@snapend

Note:
Here, you can see business logic being implemented depending on whether the device has less than 1GB of RAM or more.

---

### Use Cases

@ul
- Serve a "lite" app to users on low-end devices
- Add context to metrics
@ulend

Note:

- Enable developers to tailor content at runtime in accordance with hardware limitations. For example, developers can serve a "lite" app to users on low-end devices, resulting in better experiences and fewer frustrations.
- Add context to metrics, such as the amount of time a task takes to complete in JavaScript, through the lens of device memory. This will result in a better understanding of how device memory correlates with user behavior, conversions, or other metrics important to your business.

---?image=template/img/caniuse/device-memory.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
<a href="https://developer.mozilla.org/en-US/docs/Web/API/Navigator/deviceMemory#Browser_compatibility" target="_blank" rel="noopener noreferrer">Reference</a>
@snapend

Note:
As for the browser support, Chrome and Opera already support this API.
