# CardValidator

Verification methods about cards numbers, CVV, Expiry dates, and useful constants about card types


# CardValidator Usage

The `CardValidator` class provides methods for validating credit card information in your Android app. Here's how you can use it:

## 1. Validate a Card Number

To validate a card number, you can use the `validateCardNumber` method, isCardValid will be true if the card number is valid, and false otherwise. Here's an example:

```java
String cardNumber = "1234 5678 9012 3456";
boolean isCardValid = CardValidator.validateCardNumber(cardNumber);
```
## 2. Validate a CVV
To validate a CVV for a specific card type, you can use the validateCVV method. For example, to validate a CVV for a MasterCard. Here's an example:

```java
int cvv = 123;
CardValidator.Cards cardType = CardValidator.Cards.MASTERCARD;
boolean isCVVValid = CardValidator.validateCVV(cvv, cardType);
```
