---?image=template/meme/lazy_loading.jpg&size=auto 100%

Note:
So, have you ever written JavaScript to enable infinite scrolling or to lazy-load images that appear below the fold?

If you're like me, you did this by listening for scroll events and requesting an element's `scrollTop` property or calling `getBoundingClientRect()` on an element. You forced the browser to stop everything and repeatedly recalculate the layout. You suffered. Your users suffered. It was a dark time.

Guess what? The dark times are now over! Introducing the glorious Intersection Observer API...

---

### Intersection Observer API

This API lets you know when an observed element enters or exits the browser's viewport (user's visible area of a web page).

Note:
This is a relatively new web API that provides easy-to-use, efficient tools for detecting changes to a DOM element's visibility within the browser viewport or within another element. No more reflow. No more suffering. None.

---?image=template/img/intersection-observer-demo.gif&size=auto 100%

@snap[west]
@size[2em](Demo)
@snapend

Note:
Here'a quick demo of the API in action. The top banner displays the answer to the question, "Is the green box in view?". As you can see, the API handles visibility of elements inside iframes too.

---?image=template/img/intersection-observer-threshold.gif&size=auto 100%

@snap[east]
Thresholds = <br>[0, 0.25, 0.5,<br>0.75, 1]
@snapend

Note:
But wait... There's more! The API also supports an option of specifying a list of thresholds. Your callback will be called every time the `intersectionRatio` crosses one of these values. The default value for threshold is [0], which explains the default behavior. If we change threshold to [0, 0.25, 0.5, 0.75, 1], we will get notified every time an additional quarter of the element becomes visible.

---

### Use Cases

@ul
- Lazy Loading
- Reporting of visibility of advertisements in order to calculate ad revenues
- Better Navigation Bar
- Check which feed cards are seen by user to avoid showing duplicate cards
@ulend

Note:

As for the use cases,
- You can decide whether or not to perform resource-intensive tasks (like animation) based on whether the user will see the result or not.
- Reporting of visibility is important in case of advertisements for revenue calculation.
- Imagine a navigation bar that allows you to jump between sections on a page. While you are scrolling through the page, the link to the section that's currently in the viewport can be highlighted using this API.
- You can also provide an improved user feeds experience. Check which feed cards are seen by user to avoid showing duplicate cards.

---?image=template/img/caniuse/intersection-observer.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
https://caniuse.com/#feat=intersectionobserver
@snapend

Note:
This API is already supported by major browsers like Chrome, Firefox, Edge, etc.
