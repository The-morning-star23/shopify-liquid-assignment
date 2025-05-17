# Shopify Liquid Assignment – Solution Explanation

## Task 1 – Dynamic Product Badge
- Implemented conditional badges on products using `product.price` and `product.variants.first.inventory_quantity`.
- Display "Budget Pick" badge if product price is below a threshold.
- Display "Limited Stock" badge if inventory is low.

## Task 2 – Custom Collection Filter
- Added a dropdown `<select>` to filter products by custom tags.
- Used `request.params.tag` to filter the collection dynamically on the frontend.

## Task 3 – Personalized Greeting
- Used Liquid’s `now` date filter with time formatting (`'%H'`) to detect current hour.
- Rendered personalized greetings based on the time of day (morning, afternoon, evening).

## Task 4 – Cart Upsell Recommendation
- Calculated cart total price using `cart.total_price`.
- Displayed a random product from the “accessories” collection if cart total is below $1000.
- Displayed a random product from the “premium” collection if cart total is $1000 or more.
- Used `shuffle` and `first` filters to pick a random product safely.

## Preview Link
https://my-liquid-test-store.myshopify.com/?pb=0
