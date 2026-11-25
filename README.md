# Moorpankh — saree storefront

A single-page static storefront. No build step: open `index.html`, or serve the folder with any static host.

- `index.html` — all markup, styles and scripts
- `img/` — photos
- `video/` — reels

## Receiving orders

The checkout collects delivery details and a payment choice (Cash on Delivery or bank transfer). It does not process payments and has no server.

To receive orders, set one or both of these near the checkout code in `index.html`:

```js
const ORDER_WHATSAPP=''; // country code + number, digits only
const ORDER_EMAIL='';
```

Until one is set, the confirmation screen tells the shopper the order has not been sent.
