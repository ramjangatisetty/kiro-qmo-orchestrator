# Functional Tests

## Overview

This document contains positive test scenarios that validate core functionality and expected system behavior. These tests ensure the system meets its functional requirements under normal operating conditions.

**Total Functional Tests:** 5

## Test Execution Notes

- Execute tests in the order presented
- Verify all preconditions before starting each test
- Document any deviations from expected results
- Report issues with clear reproduction steps

---

## Verify Acceptance Criteria: THE Flight*Search SHALL display inpu...

**Test Case ID:** SCRUM-5-TC-10035
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-0-0

### Description

This test validates the positive scenario: Test the main functionality described in: Acceptance Criteria: THE Flight*Search SHALL display input fields for origin airport, destination airport, departure date, return date optional, cabin class, and number of passengers.

### Preconditions

- System is in a stable state and ready for testing.

### Test Steps

1. **Action:** Navigate to the flight search page.
   **Expected Result:** Verify that flight search page loads successfully.

2. **Action:** Verify all required input fields are displayed origin, destination, departure date, return date, cabin class, passengers.
   **Expected Result:** Verify that all input fields are visible and labeled.

### Expected Results

- Flight search page loads successfully.
- All input fields are visible and labeled.
- Functionality works as specified in the acceptance criteria.

---

## Verify query available flights

**Test Case ID:** SCRUM-5-TC-1007e
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-2-0

### Description

This test validates the positive scenario: Test integration: query available flights.

### Preconditions

- System is in a stable state and ready for testing.

### Test Steps

1. **Action:** Interact with the flight search functionality.
   **Expected Result:** Verify that the functionality should work as specified in the acceptance criteria.

2. **Action:** Verify the functionality meets the acceptance criteria requirements.
   **Expected Result:** Verify that all acceptance criteria are satisfied.

### Expected Results

- The functionality should work as specified in the acceptance criteria.
- All acceptance criteria are satisfied.
- Functionality works as specified in the acceptance criteria.

---

## Verify a user selects a departure date, THE Flight*Search SHALL ...

**Test Case ID:** SCRUM-5-TC-10120
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-1

### Description

This test validates the positive scenario: Test the main functionality described in: WHEN a user selects a departure date, THE Flight*Search SHALL enforce that the return date if provided is after the departure date.

### Preconditions

- User is authenticated and has appropriate permissions.

### Test Steps

1. **Action:** Enter valid search criteria in all required fields.
   **Expected Result:** Verify that search criteria is accepted and validated.

2. **Action:** Click the search button to execute the search.
   **Expected Result:** Verify that search is executed and results are returned.

3. **Action:** Verify the functionality meets the acceptance criteria requirements.
   **Expected Result:** Verify that all acceptance criteria are satisfied.

### Expected Results

- Search criteria is accepted and validated.
- Search is executed and results are returned.
- All acceptance criteria are satisfied.
- Functionality works as specified in the acceptance criteria.

---

## Verify a user submits the search form with valid inputs, THE Fli...

**Test Case ID:** SCRUM-5-TC-10234
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-2

### Description

This test validates the positive scenario: Test the main functionality described in: WHEN a user submits the search form with valid inputs, THE Flight*Search SHALL query available flights and navigate to the Search*Results page.

### Preconditions

- User is authenticated and has appropriate permissions.
- User interface is loaded and accessible.

### Test Steps

1. **Action:** Enter valid search criteria in all required fields.
   **Expected Result:** Verify that search criteria is accepted and validated.

2. **Action:** Click the search button to execute the search.
   **Expected Result:** Verify that search is executed and results are returned.

3. **Action:** Verify the functionality meets the acceptance criteria requirements.
   **Expected Result:** Verify that all acceptance criteria are satisfied.

### Expected Results

- Search criteria is accepted and validated.
- Search is executed and results are returned.
- All acceptance criteria are satisfied.
- Functionality works as specified in the acceptance criteria.

---

## Verify query available flights

**Test Case ID:** SCRUM-5-TC-1027e
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-2

### Description

This test validates the positive scenario: Test integration: query available flights.

### Preconditions

- System is in a stable state and ready for testing.

### Test Steps

1. **Action:** Interact with the flight search functionality.
   **Expected Result:** Verify that the functionality should work as specified in the acceptance criteria.

2. **Action:** Verify the functionality meets the acceptance criteria requirements.
   **Expected Result:** Verify that all acceptance criteria are satisfied.

### Expected Results

- The functionality should work as specified in the acceptance criteria.
- All acceptance criteria are satisfied.
- Functionality works as specified in the acceptance criteria.

---

*Generated automatically from Jira acceptance criteria. Focus on positive scenarios and core functionality validation.*
