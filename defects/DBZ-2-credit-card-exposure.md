# DBZ-2 — Full Credit Card Number Displayed in Purchase Confirmation

## Summary

After a successful checkout, DemoBlaze displayed the complete test credit-card value in the purchase confirmation.

## Priority

High

## Type

Functional defect / sensitive data exposure

## Preconditions

- At least one product is present in the cart.
- The checkout form is open.

## Steps to Reproduce

1. Enter a valid customer name.
2. Enter a non-empty test credit-card value.
3. Select **Purchase**.
4. Review the purchase confirmation.

## Expected Result

The complete credit-card value should not be displayed in the confirmation. Payment information should be omitted or masked.

## Actual Result

The purchase confirmation displayed the full test credit-card value entered during checkout.

## Reproducibility

Reproduced during manual checkout testing.

## Environment

- DemoBlaze web application
- Google Chrome
- Windows 11

## Test Reference

Failed Qase test case: **Verify Full Credit Card Data Is Not Exposed**

> Note: The public portfolio intentionally does not reproduce the full test-card value used during execution.
