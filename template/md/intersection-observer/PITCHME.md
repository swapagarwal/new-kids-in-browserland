### Intersection Observer API

(A modern solution to handle scroll events!)

@ul
- This API allows you to fire a callback function when an element enters the viewport (user's visible area of a web page).
@ulend

---

### Demo

![Demo of Intersection Observer API](template/img/intersection-observer-demo.gif)

---

### Demo  (Continued)

![Another Demo of Intersection Observer API](template/img/intersection-observer-threshold.gif)

---

### Use Cases

@ul
- Lazy-loading
- Infinite scrolling
- Report ad visibility
- Nav bar
- Better user feed
@ulend

Note:

- Lazy-loading of images or other content as a page is scrolled. Deciding whether or not to perform tasks or animation processes based on whether or not the user will see the result.
- Implementing "infinite scrolling" web sites, where more and more content is loaded and rendered as you scroll, so that the user doesn't have to flip through pages.
- Reporting of visibility of advertisements in order to calculate ad revenues.
- Imagine a navigation bar that allows you to jump between sections on a page. When scrolling, the link to the section that's currently in the viewport should be highlighted.
- Check which feed cards are seen by user to avoid showing duplicate cards.
