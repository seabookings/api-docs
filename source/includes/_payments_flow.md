# Payment flows
The activity settings will dictate how the payment flow is done.

## Policies
When invoking one of the activities APIs, the settings block will return a group of properties that dictate how to make a booking and how to perform a payment.

```
"settings": {
    "comission_percentage": 0.2,
    "payment_policy": "full_amount",
    "booking_strategy": "indirect",
    "merchant_id": "acct_19S93eBFHEM5ipEo"
}
```
## Comission Percentage
The comission percentage will tell how much do we SB charge on this reservation total for this activity.
The payment policy property will tell if for this activity we should charge the full ammount or just the deposit.

## Payment policy
If the payment policy is `full_amount` we charge the total amount for the reservation and we have to specify the application_fee using the StripeConnect payment method. You should create the source in the name of `merchant_id` and use destination fees using SB publishable key.

If the payment policy is `deposit` we charge only the deposit value (`total_cents * comission_percentage`) and we use normal stripe checkout.

## Booking strategy
The `boooking_strategy` property tells how the flow of booking is. If the flow is `indirect` it means that after the payment is complete the booking will change its status to `waiting_for_confirmation`. The MTO will have to manually confirm or reject the booking (he was 4 hours to confirm/reject). Only after that we will send the confirmation/cancelation email. During that period a page should be displayed informing the customer that the availability will be confirmed. ToS and Cancelation policy links should also be displayed again.

If the flow is `instant` the confirmation page should be displayed and the booking status must be `booked`.
****

## Flows

### Global Payment flow

![Payment flow](payment_flow.svg "Payment flow")


### Stripe Checkout flow

![Checkout flow](checkout.svg "Checkout flow")


### Stripe Connect flow

![Connect flow](connect.svg "Connect flow")
