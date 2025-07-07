# OddiBites - Nairobi Street Food Delivery

A single-page web application for OddiBites, a Nairobi-based street food vendor specializing in fried chicken, juice, smokies, beef smokies, samosa, and chapatis. Customers can order via WhatsApp for fast delivery within Nairobi.

---

## Behavior Driven Development (BDD) Documentation

### Feature: Online Food Ordering via WhatsApp

#### As a customer
I want to view the OddiBites menu, select items, and place an order via WhatsApp
So that I can get my favorite street food delivered to my location in Nairobi.

---

#### Scenario 1: Viewing the Menu
- **Given** I am a visitor to the OddiBites website
- **When** the page loads
- **Then** I should see a list of menu items with images, descriptions, and prices

#### Scenario 2: Adding Items to Cart
- **Given** I am viewing the menu
- **When** I select a quantity and click "Add to Cart" for an item
- **Then** the item should appear in my cart with the correct quantity and price
- **And** the cart total should update accordingly

#### Scenario 3: Modifying the Cart
- **Given** I have items in my cart
- **When** I increase or decrease the quantity of an item
- **Then** the cart should update the item quantity and total price
- **When** I remove an item
- **Then** it should disappear from the cart and the total should update

#### Scenario 4: Placing an Order via WhatsApp
- **Given** I have at least one item in my cart
- **When** I click "Send Order via WhatsApp"
- **Then** a WhatsApp message should be generated with my order details and total
- **And** WhatsApp should open (in a new tab or app) ready to send the message to OddiBites
- **And** my cart should be cleared and the page refreshed after order submission

#### Scenario 5: Empty Cart Handling
- **Given** my cart is empty
- **When** I try to place an order
- **Then** I should see an alert that my cart is empty and the order is not sent

#### Scenario 6: Accessibility and Responsiveness
- **Given** I am using any device (mobile, tablet, desktop)
- **When** I interact with the site
- **Then** the layout and controls should be usable and accessible

---

## Deployment
This site is deployed via GitHub Pages at: [https://oddibites.github.io/](https://oddibites.github.io/)

## License
MIT
