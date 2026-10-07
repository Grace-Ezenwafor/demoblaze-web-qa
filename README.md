# DemoBlaze Web QA

End-to-end manual QA portfolio project for the DemoBlaze e-commerce web application.

## Project Overview

This project demonstrates a practical QA workflow from requirements analysis through test design, execution, defect reporting, and traceability.

The testing work was completed as a portfolio/training project using defined acceptance criteria for the selected DemoBlaze features.

## Features Covered

- Authentication
  - Sign Up
  - Login
- Cart
- Checkout

## QA Activities Performed

- Requirements analysis
- Risk identification
- Test scenario and test case design
- Positive and negative testing
- Manual test execution
- Regression and retesting concepts
- Defect investigation
- Jira bug reporting
- Test management and execution in Qase
- Requirements-to-test-to-defect traceability

## Tools Used

- **Qase** — test case management and manual test execution
- **Jira** — story and defect tracking
- **Chrome** — web application testing

## Test Execution Summary

### Authentication

- Test cases executed: 11
- Passed: 11
- Failed: 0

### Cart & Checkout

- Test cases executed: 17
- Passed: 15
- Failed: 2
- Blocked: 0

### Overall

- Total test cases executed: 28
- Passed: 26
- Failed: 2

## Defects Identified

### DBZ-2 — Full credit card number displayed in purchase confirmation

After a successful checkout, the purchase confirmation displayed the complete test credit-card value instead of omitting or masking it.

### DBZ-3 — Purchase completed successfully with an empty cart

The application allowed checkout to complete successfully when no products were present in the cart and displayed a successful purchase confirmation with a zero-value order.

## QA Workflow Demonstrated

```text
Jira Story
    ↓
Requirements Analysis
    ↓
Test Design
    ↓
Qase Test Cases
    ↓
Manual Test Execution
    ↓
Failed Test Investigation
    ↓
Jira Defect
    ↓
Traceability / Retest
```

## Repository Structure

```text
demoblaze-web-qa/
├── README.md
├── docs/
│   ├── requirements-analysis.md
│   └── test-strategy.md
├── test-cases/
│   └── qase-test-cases.md
├── test-execution/
│   └── execution-summary.md
├── defects/
│   ├── DBZ-2-credit-card-exposure.md
│   └── DBZ-3-empty-cart-purchase.md
└── screenshots/
    ├── qase/
    └── jira/
```

The supporting documentation and sanitized evidence will be added progressively as the project is packaged for the portfolio.

## Career Direction

This project is part of my progression from strong manual QA fundamentals toward **QA Automation Engineering**, with SQL/database testing, API testing, TypeScript, Playwright, Git/GitHub, and CI/CD forming the next stages of the learning path.
