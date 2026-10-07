# Qase Test Case Summary

## Purpose

This document summarizes the manual test coverage designed and managed in Qase for the DemoBlaze QA portfolio project. Detailed preconditions, test data, steps, and expected results were maintained in Qase during execution.

## Authentication — Sign Up

| Test Case | Priority | Behavior | Result |
|---|---|---|---|
| Create Account with Unique Credentials | High | Positive | Passed |
| Attempt Sign Up with Existing Username | High | Negative | Passed |
| Attempt Sign Up with Blank Username | Medium | Negative | Passed |
| Attempt Sign Up with Blank Password | Medium | Negative | Passed |
| Attempt Sign Up with Both Username and Password Blank | Medium | Negative | Passed |

## Authentication — Login

| Test Case | Priority | Behavior | Result |
|---|---|---|---|
| Log In with Valid Registered Credentials | High | Positive | Passed |
| Attempt Login with Registered Username and Incorrect Password | High | Negative | Passed |
| Attempt Login with Unregistered Username | High | Negative | Passed |
| Attempt Login with Blank Username | Medium | Negative | Passed |
| Attempt Login with Blank Password | Medium | Negative | Passed |
| Attempt Login with Both Username and Password Blank | Medium | Negative | Passed |

### Authentication Result

- Total executed: 11
- Passed: 11
- Failed: 0

## Cart

| Test Case | Result |
|---|---|
| Add a Single Product to the Cart | Passed |
| Add Multiple Different Products to the Cart | Passed |
| Add the Same Product Twice to the Cart | Passed |
| Verify Cart Item Name and Price | Passed |
| Verify Cart Total for Multiple Products | Passed |
| Remove a Product and Verify Cart Total Updates | Passed |
| Remove the Last Product from the Cart | Passed |
| Verify Cart Contents Persist After Page Refresh | Passed |

## Checkout

| Test Case | Result |
|---|---|
| Open the Checkout Form from the Cart | Passed |
| Attempt Purchase with Name Blank | Passed |
| Attempt Purchase with Credit Card Blank | Passed |
| Attempt Purchase with Both Required Fields Blank | Passed |
| Complete Purchase with Required Fields Supplied | Passed |
| Verify Purchase Confirmation Information | Passed |
| Verify Full Credit Card Data Is Not Exposed | **Failed** |
| Verify Cart Is Cleared After Successful Purchase | Passed |
| Attempt Purchase with an Empty Cart | **Failed** |

### Cart & Checkout Result

- Total executed: 17
- Passed: 15
- Failed: 2
- Blocked: 0

## Overall Result

- Total executed: 28
- Passed: 26
- Failed: 2
- Blocked: 0

The two failed test cases resulted in Jira defect reports DBZ-2 and DBZ-3.
