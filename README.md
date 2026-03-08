# Shopping Cart with Object Oriented JavaScript

## Overview
This project recreates a shopping cart using the Object Oriented JavaScript (OOJ) approach and DOM manipulation.

It covers:
- Product modeling with classes
- Cart item modeling with quantity and total calculation
- Cart management (add, remove, total, display)
- UI interactions for quantity updates, delete, and like/unlike

## Checkpoint Requirements Mapping

### 1. Product class
`Product` stores:
- `id`
- `name`
- `price`

Additional UI fields used in this project:
- `quantity`
- `heart`
- `description`
- `image`

### 2. Shopping cart item class
`ShoppingCartItem` stores:
- `product`
- `quantity`

### 3. Item total price method
`ShoppingCartItem.calculateTotalPrice()` returns:
- `product.price * quantity`

### 4. Shopping cart class
`Shoppingcart` contains:
- `items` (array of `ShoppingCartItem`)

Methods implemented:
- `getTotalPrice()` -> total of all cart items
- `addItem(product)` -> add product or increase quantity
- `removeItem(productId)` -> decrease quantity or remove item at 0
- `clearItem(productId)` -> delete item from cart
- `displayCartItems()` -> render cart in the DOM
- `toggleLike(productId)` -> like/unlike item

## Testing the Required Abilities

The app demonstrates:
1. Creating products (`new Product(...)`)
2. Creating a shopping cart (`new Shoppingcart(...)`)
3. Adding items to the cart (`addItem`)
4. Displaying the cart (`displayCartItems`)
5. Removing an item from the cart (`removeItem` / `clearItem`)

## Project Structure

- `index (1).html` -> page structure
- `app.js` -> OO logic + DOM behavior
- `style/style.css` -> cart styling and like color state
- `assets/` -> product images

## How to Run

1. Open `index (1).html` in a browser.
2. Use the controls on each product card:
- `+` to increase quantity
- `-` to decrease quantity
- trash icon to remove item
- heart icon to like/unlike (color change)

The total price updates automatically after each action.
