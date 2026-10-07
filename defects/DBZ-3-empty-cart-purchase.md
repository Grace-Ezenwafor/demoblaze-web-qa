# DBZ-3 — Purchase Can Be Completed Successfully with an Empty Cart

## Summary

DemoBlaze allowed checkout to complete successfully while the cart contained no products.

## Priority

High

## Type

Functional defect

## Preconditions

- DemoBlaze is accessible.
- The cart contains no products.
- The Cart page is open.

## Steps to Reproduce

1. Open the Cart page with no products in the cart.
2. Select **Place Order**.
3. Enter a valid Name.
4. Enter a non-empty test Credit Card value.
5. Select **Purchase**.
6. Observe the result.

## Expected Result

The purchase should not complete successfully when the cart is empty, and no successful purchase confirmation should be generated.

## Actual Result

The purchase completed successfully with an empty cart. A purchase confirmation was displayed with an order ID and an amount of 0 USD.

## Reproducibility

Reproduced during manual checkout testing.

## Environment

- DemoBlaze web application
- Google Chrome
- Windows 11

## Test Reference

Failed Qase test case: **Attempt Purchase with an Empty Cart**
