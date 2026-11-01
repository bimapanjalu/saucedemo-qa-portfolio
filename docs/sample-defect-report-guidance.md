# Guidance: Writing a Credible Defect Report

This repository does not include a fabricated “confirmed bug.” A bug report is evidence of an observed deviation, so it should only be created after reproduction.

## Before reporting

1. Re-run the same steps from a clean state.
2. Confirm the expected behavior from a requirement or clearly stated test expectation.
3. Record the browser, OS, test account type, and date.
4. Capture the exact actual result.
5. Check whether the issue is caused by test setup, network conditions, or stale session state.
6. If it is not reproducible, document that fact instead of presenting it as confirmed.

## Good versus weak wording

**Weak:** “Checkout is broken.”

**Better:** “With a cart containing one item, submitting the checkout form with the required First Name field blank produced `[actual observed behavior]` in `[browser/version]` on `[date]`.”

The bracketed content must be replaced with a real observation before the report is published.
