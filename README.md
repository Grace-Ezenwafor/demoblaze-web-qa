# DemoBlaze Web QA

End-to-end manual QA portfolio project for the DemoBlaze e-commerce web application.

## Project Overview

This project demonstrates a practical QA workflow from requirements analysis through test design, execution, defect investigation, Jira reporting, and traceability.

The work was completed as a portfolio/training project using defined acceptance criteria for selected DemoBlaze features.

## Features Covered

- Authentication
  - Sign Up
  - Login
- Cart
- Checkout

## Tools Used

- **Qase** — test case management and manual test execution
- **Jira** — story and defect tracking
- **Google Chrome** — web application testing
- **GitHub** — public portfolio documentation

## Portfolio Artifacts

- [Requirements Analysis](docs/requirements-analysis.md)
- [Test Strategy](docs/test-strategy.md)
- [Qase Test Case Summary](test-cases/qase-test-cases.md)
- [Test Execution Summary](test-execution/execution-summary.md)
- [DBZ-2 — Full Credit Card Number Displayed in Purchase Confirmation](defects/DBZ-2-credit-card-exposure.md)
- [DBZ-3 — Purchase Can Be Completed Successfully with an Empty Cart](defects/DBZ-3-empty-cart-purchase.md)

## Test Execution Results

| Area | Executed | Passed | Failed | Blocked |
|---|---:|---:|---:|---:|
| Authentication | 11 | 11 | 0 | 0 |
| Cart & Checkout | 17 | 15 | 2 | 0 |
| **Overall** | **28** | **26** | **2** | **0** |

## Confirmed Defects

### DBZ-2 — Full credit card number displayed in purchase confirmation

After a successful checkout, the purchase confirmation displayed the complete test credit-card value instead of omitting or masking it.

**Status:** Open / requires resolution and retesting.

### DBZ-3 — Purchase completed successfully with an empty cart

The application allowed checkout to complete successfully when no products were present in the cart and generated a successful zero-value purchase confirmation.

**Status:** Open / requires resolution and retesting.

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
Failure Investigation
    ↓
Jira Defect Reporting
    ↓
Traceability
    ↓
Retest after fix
```

## Evidence & Privacy

The original testing work was managed in Qase and Jira. This GitHub repository is the public portfolio record, so the important project evidence is documented here in a recruiter-accessible format.

Sensitive-looking test data is intentionally not reproduced in the public defect documentation. In particular, the full test credit-card value used during execution is omitted.

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
└── defects/
    ├── DBZ-2-credit-card-exposure.md
    └── DBZ-3-empty-cart-purchase.md
```

## Career Direction

This project is part of my progression from strong manual QA fundamentals toward **QA Automation Engineering**. The next stages of my portfolio will add SQL/database testing, API testing, TypeScript, Playwright, Git workflows, and CI/CD as those skills are completed.
