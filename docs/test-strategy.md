# Test Strategy

## Project

DemoBlaze E-commerce Web Application

## Objective

The objective of this testing effort was to validate selected core user flows of the DemoBlaze web application and identify functional defects that could affect account access, cart behaviour, and checkout.

The project focused on practical manual QA activities including requirements analysis, test design, test execution, defect reporting, and traceability.

---

## Features in Scope

### Authentication
- Sign Up
- Login

### Cart
- Add product to cart
- Add multiple products
- Add duplicate products
- Verify product details
- Cart total calculation
- Remove products
- Cart persistence after refresh

### Checkout
- Open checkout form
- Required-field validation
- Successful checkout
- Purchase confirmation
- Credit-card data exposure
- Post-purchase cart state
- Empty-cart checkout

---

## Out of Scope

The following areas were not part of the core testing scope:

- Real payment processing
- Credit-card format validation
- Luhn validation
- Payment gateway integration
- Performance testing
- Load testing
- Full security penetration testing
- Backend/API validation
- Database validation
- Full cross-browser compatibility testing
- Mobile application testing

These areas may be covered in future QA projects as the portfolio expands into API, database, and automation testing.

---

## Test Types Used

- Functional testing
- Positive testing
- Negative testing
- Exploratory testing
- Regression testing concepts
- Retesting concepts
- Boundary and validation-focused testing

---

## Test Design Approach

Test coverage was created from defined requirements and acceptance criteria.

The process followed:

1. Review requirements.
2. Identify unclear or missing behaviour.
3. Identify business and user risks.
4. Define test scenarios.
5. Create detailed test cases.
6. Organize reusable cases in Qase.
7. Execute cases in structured test runs.
8. Investigate failures.
9. Report confirmed defects in Jira.

AI-assisted tools were used to speed up repetitive test-case drafting, while final test coverage and expected results were reviewed before execution.

---

## Test Environment

- Application: DemoBlaze Web Application
- Testing type: Manual web testing
- Operating system: Windows 11
- Browser: Google Chrome
- Test management: Qase
- Defect tracking: Jira

---

## Entry Criteria

Testing could begin when:

- The DemoBlaze application was accessible.
- Test requirements and expected behaviour had been defined.
- Test cases were prepared in Qase.
- Required test data was available.

---

## Exit Criteria

Testing was considered complete when:

- All planned test cases had been executed.
- Test results had been recorded.
- Failed cases had been investigated.
- Confirmed defects had been documented in Jira.
- Testing results had been summarized.

---

## Execution Results

### Authentication
- 11 test cases executed
- 11 passed
- 0 failed

### Cart & Checkout
- 17 test cases executed
- 15 passed
- 2 failed

### Overall
- 28 test cases executed
- 26 passed
- 2 failed

---

## Defect Summary

Two confirmed defects were identified during Cart & Checkout testing:

1. Full credit-card number displayed in the purchase confirmation.
2. Purchase successfully completed with an empty cart.

Both defects were documented in Jira and linked to the related testing workflow.

---

## Tools

- Qase
- Jira
- Google Chrome
- GitHub
