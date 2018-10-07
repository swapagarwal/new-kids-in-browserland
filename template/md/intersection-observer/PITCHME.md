### Intersection Observer API

- This API allows you to fire a callback function when an element enters the viewport (user's visible area of a web page).

---

@snap[west split-screen-img]
![Demo of Intersection Observer API](template/img/intersection-observer-demo.gif)
@snapend

@snap[east split-screen-img]
![Another Demo of Intersection Observer API](template/img/intersection-observer-threshold.gif)
@snapend

---

### Use Cases

@ul
- Lazy-loading of images or other content as a page is scrolled.
- Implementing "infinite scrolling" web sites, where more and more content is loaded and rendered as you scroll, so that the user doesn't have to flip through pages.
- Reporting of visibility of advertisements in order to calculate ad revenues.
@ulend

---

### Use Cases (Continued)

@ul
- Imagine a navigation bar that allows you to jump between sections on a page. When scrolling, the link to the section that's currently in the viewport should be highlighted.
- Deciding whether or not to perform tasks or animation processes based on whether or not the user will see the result.
- Check which feed cards are seen by user to avoid showing duplicate cards.
@ulend
