<div align="center">

# Manual QA Testing — SauceDemo

**Test design and execution documentation for a demo e-commerce workflow.**

`Manual Testing` `Test Cases` `Defect Reporting` `E-commerce`

</div>

---

## Overview

This project documents a manual QA approach for [SauceDemo](https://www.saucedemo.com/), a public demo application intended for practice. The scope covers authentication, product browsing, cart behavior, and checkout.

This repository contains **test design artifacts**. Execution results remain `NOT RUN` until you perform the checks against the current demo application. Do not present an unexecuted test plan as proof of a successful test run.

## Objectives

- Translate user-facing workflows into testable scenarios.
- Include positive, negative, and boundary-oriented checks.
- Record preconditions, steps, expected results, and actual results.
- Track defects using clear reproduction steps and evidence.
- Produce a transparent execution summary.

## Scope

### In scope
- Login with valid and invalid credentials.
- Locked-out user behavior.
- Product list and product detail navigation.
- Add/remove cart items.
- Checkout form validation.
- Completing a demo purchase.

### Out of scope
- Real payments or financial transactions.
- Production customer data.
- Load, penetration, or destructive testing.
- Claims about accessibility, browser compatibility, or security unless separately tested.

## Test environment

Record the actual environment before executing the suite.

| Field | Value |
|---|---|
| Application | SauceDemo public demo |
| URL | `https://www.saucedemo.com/` |
| Browser and version | `[fill after execution]` |
| Operating system | `[fill after execution]` |
| Test date | `[fill after execution]` |
| Tester | `[your name or public handle]` |

The demo site and its behavior may change. Confirm the current page and credentials published by the demo provider before running tests. Do not use real or reused passwords.

## Test design

The full list is in [`test-cases.csv`](test-cases.csv). Execution tracking is in [`docs/test-execution-report.md`](docs/test-execution-report.md).

| Test area | Examples |
|---|---|
| Authentication | Valid login, invalid password, locked-out user |
| Catalog | Product list visibility, product details |
| Cart | Add item, remove item, badge and cart contents |
| Checkout | Required-field validation, order summary, completion confirmation |

## Execution process

1. Read the preconditions for a test case.
2. Reset the browser to a known state where needed.
3. Follow the steps in order without skipping an action.
4. Compare actual behavior with the expected result.
5. Mark `PASS`, `FAIL`, `BLOCKED`, or `NOT RUN`.
6. For a failure, preserve the exact message and create a defect report using [`docs/defect-report-template.md`](docs/defect-report-template.md).
7. Re-run the affected case after a fix or environment change and link the retest evidence.

## Defect reporting

A useful defect report includes:
- A short, specific title.
- Environment and preconditions.
- Numbered reproduction steps.
- Expected versus actual result.
- Reproducibility and impact.
- Sanitized screenshot or other evidence.
- Status and retest result.

Use [`docs/sample-defect-report-guidance.md`](docs/sample-defect-report-guidance.md) to avoid reporting an unverified issue as a real defect.

## Results

**Current execution status: NOT RUN.**

The repository is ready for execution, but this pack does not claim that the current demo site has been tested. Update the report only after you perform the test cases. Include the date, browser, results, evidence, and any limitations.

## Deliverables

- `test-plan.md` — scope, approach, environment, and exit criteria.
- `test-cases.csv` — structured manual test cases.
- `test-execution-report.md` — status tracking.
- `defect-report-template.md` — reusable defect template.
- `sample-defect-report-guidance.md` — rules for creating valid bug reports.

## Next improvements

- Execute all cases and attach sanitized screenshots.
- Add boundary and exploratory tests based on observed behavior.
- Compare manual cases with the Playwright automation suite.
- Add a short retrospective describing what the testing did and did not cover.
