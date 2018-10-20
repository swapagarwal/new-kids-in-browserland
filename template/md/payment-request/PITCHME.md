### Payment Request API

(Buy seamlessly on the web!)

@ul
- This API is meant to reduce the number of steps needed to complete a payment online, potentially doing away with (long) checkout forms.
@ulend

---

### Demo

![Demo without Payment Request API](template/img/payment-request-without.png)

---

### Demo (Continued)

![Demo with Payment Request API](template/img/payment-request-demo.png)

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
