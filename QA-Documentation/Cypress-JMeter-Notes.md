# Cypress and JMeter — Setup Notes

The uploaded archive did not include a reliable, ready-to-run Cypress suite or a JMeter `.jmx` test plan. This note intentionally avoids claiming those tools were already executed.

## Cypress starter setup
1. Install Node.js in your local project environment.
2. From a separate QA workspace, run `npm init -y` and install Cypress with `npm install --save-dev cypress`.
3. Configure a local base URL and stable selectors for the actual application.
4. Implement tests for registration, login, booking, logout, and admin access; use synthetic accounts only.
5. Save screenshots/videos only when useful, and check them for personal data before committing.

## JMeter performance test
1. Use Apache JMeter on a local or explicitly authorized staging system only.
2. Set up Thread Group, HTTP Request Defaults, HTTP Request, timers, and listeners.
3. Start with a small baseline (for example, a few virtual users) and increase gradually.
4. Record thread count, ramp-up, duration, response time, throughput, and error rate.
5. Do not upload session cookies, authentication tokens, real user data, or sensitive `.jmx` properties.

Record the actual configuration and results before stating performance or automation outcomes in a CV or README.
