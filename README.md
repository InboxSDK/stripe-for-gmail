# stripe-for-gmail
A gmail extension that shows customers stripe information alongside the emails they send you

Get It Here:
------------
Hosted on the chrome web store here: https://chrome.google.com/webstore/detail/stripe-for-gmail/dhnddbohjigcdbcfjdngilgkdcbjjhna (you must be logged into stripe in the same browser)

What It Does:
-------------
1. Adds indicators to your inbox to show you which emails are from customers in your stripe account.
2. When reading an email conversation, the sidebar populates with information about the customer in stripe like how much they've been charged total, recent subscriptions, invoices and payments.

![indicators](/images/stripe1.webp "Indicators")

![sidebar](/images/stripe2.webp "Sidebar")

How It Works:
-------------
The extension assumes you are logged into Stripe and makes authenticated requests to the Stripe servers. It doesn't use the official API but instead makes the same ajax requests that the Stripe website does. This is because Stripe hasn't yet officially published their /search API which lets you find customers by their email address. Once this is available, I'll modify this extension to use the official API and use OAuth to authenticate.
