# Test Plan — Movie Nation

## Objective
Assess core user workflows, admin workflows, data validation, session behavior, and basic performance risks.

## In scope
- Registration: required fields, duplicate/invalid input, password handling
- Login/logout: valid/invalid credentials, session termination, direct URL access
- Movie browsing and timetable selection
- Seat selection, booking totals, and payment-summary consistency
- Admin access and content-management forms
- Basic load/performance behavior on a local test environment

## Test approach
1. Prepare a local database with synthetic test data only.
2. Run manual functional and negative tests from `Manual-Test-Cases.md`.
3. Record evidence (screenshots, environment, steps, expected/actual results) without real user data.
4. If configured, automate stable flows with Cypress and run a controlled JMeter test against a local/staging environment.
5. Record actual results and defects; do not run load tests against systems without permission.

## Entry criteria
- Local test environment is isolated and configured.
- Synthetic accounts and records are available.
- Test environment URL and test data are documented.

## Exit criteria
- All planned cases have a recorded status.
- Critical defects are reported and retested.
- Any unexecuted or blocked tests are clearly identified.

## Risks
- Legacy source includes plaintext password storage and SQL-injection-prone queries.
- Original media assets were excluded from this public package.
- The included database export has schema only, so test data must be created locally.
