---?image=template/meme/my-name-is-yu.jpg&size=auto 100%

Note:
To provide a sophisticated user experience, it's important to help users authenticate themselves to your website. Authenticated users can interact with each other using a dedicated profile, sync data across devices, or process data while offline; the list goes on and on. But creating, remembering and typing passwords tends to be cumbersome for end-users, especially on mobile screens. It can even lead them to re-using the same passwords on different sites, which, of course, is a security risk.

---

### Credential Management API

This API lets a website store and retrieve password credentials.

Note:
Enter the Credential Management API. It gives developers programmatic access to a browser's credential manager and helps users sign-in more easily.

---?image=template/img/carbon/credential-management.png&size=95% auto

@snap[north]
@size[1.5em](API Spec)
@snapend

Note:
Here are the API specifications. The first 3 are simple CRUD operations. The last one is a bit interesting. When you call `preventSilentAccess`, the browser ensures that user mediation is required on the next credential access request, effectively "logging out" the user.

---?image=template/img/credential-management-demo.gif&size=auto 90%

@snap[west]
@size[2em](Demo)
@snapend

Note:
Let's take a look at a user flow after integrating with this API.
The user visits the website. Notice the bottom blue banner to see how the site attempts to sign-in the user automatically. Note that this would work seamlessly only when the `preventSilentAccess` is set to `false`.

---

### Use Cases

@ul
- Removes friction from sign-in flows
- One tap sign-in with account chooser
- Stores and syncs credentials
@ulend

Note:

- The most exciting part of using Credential Management API is the auto sign-in. Users can be automatically signed back into a site even if their session has expired or they saved credentials on another device.
- Allows one tap sign in with account chooser - Users are presented with a native account chooser.
- Your application can store either a username and password combination or even federated account details. These credentials can be synced across devices by the browser.

---?image=template/img/caniuse/credential-management.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
https://caniuse.com/#feat=credential-management
@snapend

Note:
This is supported on UC and Chrome browsers, which account for more than 70% combined usage in India.
