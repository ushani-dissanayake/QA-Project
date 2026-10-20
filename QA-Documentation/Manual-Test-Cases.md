# Manual Test Cases — Movie Nation

These are planned test cases, not a claim that execution has already occurred. Fill in the **Actual Result**, **Status**, and **Evidence** columns after testing.

| ID | Area | Test | Expected result | Actual result / Status |
|---|---|---|---|---|
| TC-REG-01 | Registration | Submit valid synthetic user details | Account is created and confirmation/next step is shown | Not executed |
| TC-REG-02 | Registration | Submit with required fields empty | Validation prevents submission and explains required fields | Not executed |
| TC-REG-03 | Registration | Submit invalid email format | Invalid email is rejected | Not executed |
| TC-REG-04 | Registration | Submit mismatched password and confirmation | Submission is rejected with a clear validation message | Not executed |
| TC-LOG-01 | Login | Sign in with a valid synthetic account | User is authenticated and reaches the expected page | Not executed |
| TC-LOG-02 | Login | Sign in with an incorrect password | Access is denied without exposing submitted credentials | Not executed |
| TC-LOG-03 | Login | Enter SQL metacharacters in login fields | Input is handled safely; authentication is not bypassed | Not executed |
| TC-SES-01 | Session | Log out and use browser back/direct protected URL | Protected content is not accessible after logout | Not executed |
| TC-MOV-01 | Movies | Open movie listing and select a movie | Correct movie details are displayed | Not executed |
| TC-TIME-01 | Timetable | Select a showtime | Selected movie/time remains consistent on the next step | Not executed |
| TC-SEAT-01 | Seats | Select and deselect available seats | Selection state and price total update correctly | Not executed |
| TC-SEAT-02 | Seats | Attempt to select an already booked seat | Seat cannot be double-booked | Not executed |
| TC-BOOK-01 | Booking | Review ticket summary | Movie, showtime, seat count, and total are consistent | Not executed |
| TC-ADM-01 | Admin | Open admin page without authentication | Access is denied or redirected to login | Not executed |
| TC-ADM-02 | Admin | Attempt admin login with invalid credentials | Access is denied | Not executed |
| TC-PERF-01 | Performance | Run a small, authorized baseline against movie listing | Response times and errors are recorded; no unexplained failures | Not executed |
