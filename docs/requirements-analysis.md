# Requirements Analysis

## Project

DemoBlaze E-commerce Web Application

## Purpose

This document records the requirements analysis performed before designing and executing test cases for the selected DemoBlaze features.

The objective was to identify expected behaviour, unclear requirements, business risks, and appropriate test coverage before execution.

---

# Authentication

## Features Reviewed

- Sign Up
- Login

## Key Testing Areas

- Successful account registration
- Duplicate account registration
- Required-field validation
- Successful login with registered credentials
- Incorrect password handling
- Unregistered username handling
- Blank login credentials
- Authenticated user state

## Risks Considered

- Unauthorized access
- Incorrect authentication behaviour
- Poor validation of required fields
- Incorrect handling of registered and unregistered users
- Session/authentication state not being reflected correctly

---

# Cart & Checkout

## User Story

As a customer, I want to add products to my cart and complete an order so that I can purchase items from the store.

## Approved Requirements

1. A customer can add a product to the cart from the product-details page.
2. Products added to the cart must appear on the Cart page.
3. Multiple different products can be added to the cart.
4. Adding the same product twice creates two separate cart rows.
5. The cart total must equal the sum of the prices of the products currently in the cart.
6. Removing a product must update the cart total.
7. Clicking Place Order opens the checkout form.
8. Name and Credit Card are the required checkout fields.
9. Country, City, Month, and Year are optional for this testing scope.
10. Credit Card only needs to be non-empty for this testing scope.
11. A purchase must not complete if Name is blank.
12. A purchase must not complete if Credit Card is blank.
13. A purchase must not complete if both required fields are blank.
14. A successful purchase must display confirmation information.
15. Confirmation must contain an order ID, order amount, customer name, and purchase date.
16. Full credit-card information must not be exposed in the confirmation.
17. Purchased items must be removed from the cart after successful checkout.
18. Checkout may open with an empty cart, but a purchase must not successfully complete.
19. Guest checkout is allowed.
20. Cart contents should survive a normal page refresh within the same browser session.

---

## Questions Raised During Requirements Analysis

- How should duplicate products appear in the cart?
- Does the cart total include tax, shipping, discounts, or only item prices?
- Which checkout fields are mandatory?
- What Credit Card validation rules apply?
- What information should appear in the purchase confirmation?
- Can checkout be completed with an empty cart?
- Is login required before checkout?
- Should the cart persist after page refresh?
- Is stock or maximum quantity validation required?

These questions were clarified before final test-case design.

---

## Key Risks Identified

- Incorrect cart totals
- Orders completing without required customer information
- Duplicate purchases
- Cart being cleared at the wrong time
- Purchased products remaining in the cart
- Sensitive card information being exposed
- Empty-cart purchases being accepted
- Incorrect purchase confirmation information

---

## Test Coverage Decision

Core functional coverage was prioritised for:

- Add to Cart
- Multiple products
- Duplicate products
- Cart item information
- Cart totals
- Product removal
- Cart persistence
- Checkout form access
- Required-field validation
- Successful purchase
- Confirmation information
- Credit-card information exposure
- Post-purchase cart state
- Empty-cart checkout

Additional security, compatibility, API, performance, and advanced exploratory testing were considered outside the core scope of this project.
