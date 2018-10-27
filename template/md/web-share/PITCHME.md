### How do you add sharing functionality on a website today?

Note:
If you've ever built a website and needed the ability to share to a social network, you know that it's not as easy as it first seems. In order to add basic share functionality, you often need to include a third party script and become familiar with its API. Not to mention the fact that third party scripts can have a detrimental effect on the page load performance of your site. As you add more and more sharing links, you'll quickly start to collect a lot of scripts.

Web developers have always been jealous of the ability that native developers have that enables them to tap into the sharing capabilities of a device. Sharing between native apps on your device is so easy, but there isn't any reason why it shouldn't be easy for web developers!

---

### Web Share API

This API offers a simple way to allow websites to invoke the native sharing capabilities of the host platform.

Note:
This is where the Web Share API comes into play. It allows websites to invoke the native sharing capabilities of the host platform directly from the web. The advantages include:
- The API is simple to use.
- You can share to any installed apps, social networks, and even websites.
- And the best thing is, that It provides a uniform and familiar user-experience.

---?image=template/img/carbon/web-share.png&size=90% auto

@snap[north]
@size[1.5em](Code Sample)
@snapend

Note:
Here's a code sample for using the Web Share API. As you can see, the API is really simple and provides just one method - navigator.share(data)
where `data` can contain `title`, `text`, and `url`

---?image=template/img/web-share-demo.gif&size=auto 90%

@snap[west]
@size[2em](Demo)
@snapend

Note:
Let's take a look at a demo integration of this API. Notice the familiar way of sharing data around.

---?image=template/img/caniuse/web-share.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
https://caniuse.com/#feat=web-share
@snapend

Note:
This API is rolled out to Chrome and is in Preview mode on Safari.
