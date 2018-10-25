### Payment Request API

(Buy seamlessly on the web!)

@ul
- This API is meant to reduce the number of steps needed to complete a payment online, potentially doing away with (long) checkout forms.
@ulend

Note:

Buying things online can be a frustrating process, especially on mobile. Even if the pages are well designed, there's a lot of information required: Our contact information, shipping and billing addresses, shipping option and card details. If you've ever just given up sometimes, you're in the majority.

The Baymard Institute took an average across 37 different studies and found that 69% of shopping carts are abandoned.

Unsurprisingly, the figures are worse on mobile, where the smaller screen and lack of a physical keyboard can make input slower. The abandonment rate on mobile can be as high as 84% or more! With the rise of mobile browsing over recent years, this means the overall problem has been getting worse. For e-commerce sites, these abandoned carts are costing a huge amount of money. Business Insider estimated $4 trillion worth of merchandise would be abandoned in one year.

Thankfully, the web is fighting back against this problem. The "Web Payments" W3C Working Group has been busy working on "a revolution in payments on the web", developing new standards to help make online payments much easier.

---?image=template/img/payment-request-without.png&size=90% auto

@snap[north]
@size[2em](BEFORE)
@snapend

---?image=template/img/payment-request-demo.png&size=auto 90%

@snap[west]
@size[2em](AFTER)
@snapend

---

### Use Cases

@ul
- Fast checkout experience
- Consistent error handling
- Express checkout
@ulend

Note:

- Fast checkout experience: Users can enter their details (credit cards and shipping addresses) once into the browser and are then ready to pay for goods and services on the web. They no longer have to fill out the same details repeatedly across different sites, thereby reducing shopping-cart abandonment.
- Consistent error handling: The browser can check the validity of card numbers, and can tell the user if a card has expired (or is about to expire). The browser can automatically suggest which card to use based on past usage patterns or restrictions from the merchant (e.g, "we only accept Visa or Mastercard"), or allow the user to say which is their default/favorite card.
- Express checkout: Let the customer buy without requiring to log in first. If you like, you can collect the user's contact details using the Payment Request UI and once they have made the purchase, offer the opportunity to create an account then, for future use.

---?image=template/img/caniuse/payment-request.png&size=90% auto

@snap[north]
@size[1.5em](Browser Support)
@snapend

@snap[south]
https://caniuse.com/#feat=payment-request
@snapend
