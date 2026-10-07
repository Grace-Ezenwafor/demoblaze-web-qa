# Test Execution Summary

## Overview

Two structured manual test runs were completed in Qase for the DemoBlaze portfolio project.

| Test Run | Executed | Passed | Failed | Blocked | Result |
|---|---:|---:|---:|---:|---|
| Authentication | 11 | 11 | 0 | 0 | Passed |
| Cart & Checkout | 17 | 15 | 2 | 0 | Failed |
| **Overall** | **28** | **26** | **2** | **0** | **2 confirmed defects** |

## Authentication Run

The authentication run covered Sign Up and Login behavior, including:

- successful registration
- duplicate registration
- blank-field validation
- valid login
- incorrect password
- unregistered username
- blank login credentials

All 11 test cases passed.

## Cart & Checkout Run

The second run covered cart behavior, checkout validation, successful purchase flow, confirmation data, post-purchase state, and empty-cart checkout.

### Failed Cases

#### Verify Full Credit Card Data Is Not Exposed

**Expected:** The complete test credit-card value should not be displayed in the purchase confirmation.

**Actual:** The purchase confirmation displayed the full test credit-card value.

**Defect:** DBZ-2

#### Attempt Purchase with an Empty Cart

**Expected:** A purchase should not complete successfully when no products are in the cart.

**Actual:** The application displayed a successful purchase confirmation with an empty cart and a zero-value order.

**Defect:** DBZ-3

## QA Status

Cart & Checkout testing completed with two open defects requiring resolution and retesting.

The related Jira story remained open rather than being marked complete while the defects were unresolved.
