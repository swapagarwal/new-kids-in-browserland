### Credential Management API

(Users love simplicity!)

This API lets a website store and retrieve password credentials.

---

### API Spec

- navigator.credentials.get()
- navigator.credentials.store()
- navigator.credentials.requireUserMediation()

---

### Demo

![Demo of Credential Management API](template/img/credential-management-demo.gif)

---

### Use Cases

@ul
- Removes friction from sign-in flows - Users can be automatically signed back into a site even if their session has expired or they saved credentials on another device.
- Allows one tap sign in with account chooser - Users can choose an account in a native account chooser.
- Stores credentials - Your application can store either a username and password combination or even federated account details. These credentials can be synced across devices by the browser.
@ulend
