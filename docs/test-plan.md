# Test Plan — SauceDemo Core Shopping Flow

## 1. Purpose

Assess the core demo shopping workflow from login through checkout and provide a repeatable record of expected behavior.

## 2. Test objectives

- Verify basic authentication outcomes.
- Verify product navigation and cart state.
- Verify required checkout fields.
- Verify that a demo order can reach its completion confirmation.
- Record deviations with reproducible steps and evidence.

## 3. Scope

**Included:** login, catalog, product detail, cart, checkout form validation, order completion.

**Excluded:** real payments, security testing, load testing, backend data integrity, and production use.

## 4. Approach

Use manual functional testing. Run positive and negative cases. Restore a known state between cases where possible. Do not infer that untested browsers or devices behave the same way.

## 5. Entry criteria

- The public demo site is reachable.
- The current demo credentials are available from the demo provider.
- A supported browser is available.
- The tester has recorded the environment.

## 6. Exit criteria

- Every in-scope test has a final status or a documented blocker.
- Every failure has evidence or an explanation of why evidence could not be captured.
- High-impact failures are documented and retested if a fix becomes available.
- The execution summary states the total tests, statuses, and limitations.

## 7. Severity guide

| Severity | Definition |
|---|---|
| Critical | Core demo flow is unavailable and no reasonable workaround exists |
| High | Major in-scope workflow fails or produces materially incorrect output |
| Medium | A feature is impaired but a workaround exists |
| Low | Cosmetic or low-impact issue with limited functional effect |

Severity is a reasoned assessment for this demo, not a formal production SLA.

## 8. Risks and limitations

- Demo behavior can change without notice.
- Shared demo data or session state may affect reproducibility.
- Browser extensions, network restrictions, or cache state can affect results.
- A functional test suite does not establish security or accessibility conformance.

## 9. Reporting

Record actual outcomes in `test-execution-report.md`. Keep defect records separate and link them by test case ID. Never invent a defect merely to make the portfolio appear more substantial.
