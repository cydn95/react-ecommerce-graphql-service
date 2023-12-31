# React Ecommerce GraphQL server

## All exports

- BasketProvider
- BasketContext
- BasketConsumer
- TinyBasket
- Coupon
- parseBasketItem
- createBasketItem

## State

The state object contains:

- items (array of the product items in the basket)
- totalPrice (the total price of the basket items)
- totalPriceMinusDiscount (total price minus discount (if applied))
- totalToPay (total price - discount + shipping)
- totalQuantity (the total items including quantity)
- freeShipping (if free shipping has been granted)
- remainingUntilFreeShippingApplies (the minimum amount required for free shipping)
- metadata (additional metadata that you can set)

## Actions

- empty (empty the basket)
- addItem (add an item)
- setItems (set all the basket items in one go)
- removeItem (remove an item)
- incrementQuantityItem (increment the quantity for a given item)
- decrementQuantityItem (decrement the quantity for a given item)
- parseBasketItem (takes a product and a variant model and returns a valid basket item)
- setValidating (set the validating flag (found in state))
- setValidatingNewCoupon (set validatingNewCoupon flag (found in state))
- setCoupon (set the coupon code)
- setDiscount (set the discount item)
- setShipping (set the current shipping item)
- setMetadata (set your metadata)
- animateItem (jiggles the item in the TinyBasket)
- onReady (calls then given function when the basket is loaded and ready)

## TinyBasket

The tiny basket accepts the following props

- hideCoupon
- hideRemainingUntilFreeShipping
- ItemCmp (The component to use when rendering each basket item)
- itemImageSizes (The sizes attr for each item image. Ex: '(min-width: 900px) 1000px, 500px')
