### Web Share API

(Sharing made ridiculously easy!)

@ul
- This API offers a simple way for websites to invoke the platform's native share widget, so that you can share to any installed apps, social networks, and even websites, in a uniform and familiar way.
@ulend

Note:

If you've ever built a website and needed the ability to share to a social network, you know that it's not as easy as it first seems. In order to add basic share functionality, you often need to include a third party script and become familiar with its API. Not to mention the fact that third party scripts can have a detrimental effect on the page load performance of your site. As you add more and more sharing links, you'll quickly start to collect a lot of scripts.

As a web developer, I've always been jealous of the ability that native developers have that enables them to tap into the sharing capabilities of a device. Sharing between native apps on your device is so easy, but there isn't any reason why it shouldn't be easy for web developers!

This is where the Web Share API comes into play. It is a simple API that allows websites to invoke the native sharing capabilities of the host platform directly from the web.

---?image=template/img/carbon/web-share.png&size=90% auto

@snap[north]
@size[1.5em](Code Sample)
@snapend

Note:
- navigator.share(data)
  - `data` can contain `title`, `text`, and `url`

---?image=template/img/web-share-demo.gif&size=auto 90%

@snap[west]
@size[2em](Demo)
@snapend

---?image=template/img/caniuse/web-share.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
https://caniuse.com/#feat=web-share
@snapend
