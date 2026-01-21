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

## Verify Acceptance Criteria: THE Flight*Search SHALL display input fields

**Test Case ID:** SCRUM-5-TC-10035
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-0-0

### Description

Test the main functionality described in: Acceptance Criteria: THE Flight*Search SHALL display input fields for origin airport, destination airport, departure date, return date optional, cabin class, and number of passengers

### Preconditions

- System is in a stable state and ready for testing

### Test Steps

1. **Action:** Navigate to the flight search page
   **Expected Result:** Flight search page loads successfully

2. **Action:** Verify the following input fields are displayed and labeled correctly:
- Origin airport
- Destination airport
- Departure date
- Return date optional
- Cabin class
- Number of passengers
   **Expected Result:** All required input fields are visible and labeled correctly

### Expected Results

- Flight search page loads successfully
- All required input fields are visible and labeled correctly
- Functionality works as specified in the acceptance criteria

---

## Verify query available flights

**Test Case ID:** SCRUM-5-TC-1007e
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-2-0

### Description

Test integration: query available flights

### Preconditions

- System is in a stable state and ready for testing

### Test Steps

1. **Action:** Interact with the flight search functionality by entering valid search criteria in all required fields
   **Expected Result:** The functionality should work as specified in the acceptance criteria

2. **Action:** Click the search button to execute the search
   **Expected Result:** Search is executed, and available flight results are displayed

3. **Action:** Verify the search results meet the acceptance criteria requirements
   **Expected Result:** All acceptance criteria are satisfied

### Expected Results

- The functionality should work as specified in the acceptance criteria
- Search is executed, and available flight results are displayed
- All acceptance criteria are satisfied
- Functionality works as specified in the acceptance criteria

---

## Verify return date validation when selecting departure date

**Test Case ID:** SCRUM-5-TC-10120
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-1

### Description

Test the main functionality described in: WHEN a user selects a departure date, THE Flight*Search SHALL enforce that the return date if provided is after the departure date

### Preconditions

- User is authenticated and has appropriate permissions

### Test Steps

1. **Action:** Enter a valid departure date in the departure date field
   **Expected Result:** Departure date is accepted and validated

2. **Action:** Enter a return date that is before the selected departure date
   **Expected Result:** System displays an error message indicating the return date must be after the departure date

3. **Action:** Enter a return date that is after the selected departure date
   **Expected Result:** Return date is accepted and validated

4. **Action:** Click the search button to execute the search
   **Expected Result:** Search is executed and results are returned

### Expected Results

- Departure date is accepted and validated
- System displays an error message indicating the return date must be after the departure date
- Return date is accepted and validated
- Search is executed and results are returned
- Functionality works as specified in the acceptance criteria

---

## Verify search form submission with valid inputs

**Test Case ID:** SCRUM-5-TC-10234
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-2

### Description

Test the main functionality described in: WHEN a user submits the search form with valid inputs, THE Flight*Search SHALL query available flights and navigate to the Search*Results page

### Preconditions

- User is authenticated and has appropriate permissions
- User interface is loaded and accessible

### Test Steps

1. **Action:** Enter valid search criteria in all required fields:
- Origin airport
- Destination airport
- Departure date
- Return date if applicable
- Cabin class
- Number of passengers
   **Expected Result:** Search criteria is accepted and validated

2. **Action:** Click the search button to execute the search
   **Expected Result:** Search is executed, and available flight results are displayed

3. **Action:** Verify the search results page is displayed
   **Expected Result:** User is navigated to the Search*Results page

### Expected Results

- Search criteria is accepted and validated
- Search is executed, and available flight results are displayed
- User is navigated to the Search*Results page
- Functionality works as specified in the acceptance criteria

---

## Verify query available flights

**Test Case ID:** SCRUM-5-TC-1027e
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-2

### Description

Test integration: query available flights

### Preconditions

- System is in a stable state and ready for testing

### Test Steps

1. **Action:** Interact with the flight search functionality by entering valid search criteria in all required fields
   **Expected Result:** The functionality should work as specified in the acceptance criteria

2. **Action:** Click the search button to execute the search
   **Expected Result:** Search is executed, and available flight results are displayed

3. **Action:** Verify the search results meet the acceptance criteria requirements
   **Expected Result:** All acceptance criteria are satisfied

### Expected Results

- The functionality should work as specified in the acceptance criteria
- Search is executed, and available flight results are displayed
- All acceptance criteria are satisfied
- Functionality works as specified in the acceptance criteria

---

*Generated automatically from Jira acceptance criteria. Focus on positive scenarios and core functionality validation.*
