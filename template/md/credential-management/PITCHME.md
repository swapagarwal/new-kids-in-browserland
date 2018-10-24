### Credential Management API

(Users love simplicity!)

@ul
- This API lets a website store and retrieve password credentials.
@ulend

Note:

To provide a sophisticated user experience, it's important to help users authenticate themselves to your website. Authenticated users can interact with each other using a dedicated profile, sync data across devices, or process data while offline; the list goes on and on. But creating, remembering and typing passwords tends to be cumbersome for end-users, especially on mobile screens which leads them to re-using the same passwords on different sites. This, of course, is a security risk.

Enter the Credential Management API. It gives developers programmatic access to a browser's credential manager and helps users sign-in more easily.

---

### API Spec

- navigator.credentials.get()
- navigator.credentials.store()
- navigator.credentials.requireUserMediation()

---?image=template/img/credential-management-demo.gif&size=auto 90%

@snap[west]
@size[2em](Demo)
@snapend

---

### Use Cases

@ul
- Removes friction from sign-in flows
- One tap sign-in with account chooser
- Stores and syncs credentials
@ulend

Note:

- Removes friction from sign-in flows - The most exciting part of using Credential Management API is the auto sign-in. Users can be automatically signed back into a site even if their session has expired or they saved credentials on another device.
- Allows one tap sign in with account chooser - Users can choose an account in a native account chooser.
- Stores credentials - Your application can store either a username and password combination or even federated account details. These credentials can be synced across devices by the browser.
