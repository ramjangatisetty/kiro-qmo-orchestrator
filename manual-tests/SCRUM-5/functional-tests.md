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

## Verify Acceptance Criteria: THE Flight*Search SHALL display input fields for origin airport, destination airport, departure date, return date optional, cabin class, and number of passengers

**Test Case ID:** SCRUM-5-TC-10035
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-0-0

### Description

Test the main functionality described in: Acceptance Criteria: THE Flight*Search SHALL display input fields for origin airport, destination airport, departure date, return date optional, cabin class, and number of passengers

### Preconditions

- System is in a stable state and ready for testing
- User is authenticated and has appropriate permissions
- User interface is loaded and accessible

### Test Steps

1. **Action:** Navigate to the flight search page by clicking the 'Flight Search' link in the main navigation menu
   **Expected Result:** Flight search page loads successfully within 3 seconds

2. **Action:** Verify the following input fields are displayed on the page:
- 'Origin Airport' field
- 'Destination Airport' field
- 'Departure Date' field
- 'Return Date' field optional
- 'Cabin Class' dropdown
- 'Number of Passengers' field
   **Expected Result:** All required input fields are visible, enabled, and labeled correctly

3. **Action:** Verify no error messages or validation issues are present on the page
   **Expected Result:** Page is free of errors and ready for user input

### Expected Results

- Flight search page loads successfully within 3 seconds
- All required input fields are visible, enabled, and labeled correctly
- Page is free of errors and ready for user input
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
- User is authenticated and has appropriate permissions
- User interface is loaded and accessible

### Test Steps

1. **Action:** Navigate to the flight search page
Enter valid data in all required fields:
- Origin Airport: 'JFK'
- Destination Airport: 'LAX'
- Departure Date: '2023-06-15'
- Return Date: '2023-06-20' optional
- Cabin Class: 'Economy'
- Number of Passengers: '2'
Click the 'Search Flights' button
   **Expected Result:** Flight search is executed, and results are displayed on the 'Search Results' page

2. **Action:** Verify the search results meet the following acceptance criteria:
- Results are displayed in a clear and organized manner
- All required flight details are shown airline, flight times, duration, stops, etc.
- Sorting and filtering options are available
- Pricing information is accurate and up-to-date
   **Expected Result:** All acceptance criteria for the flight search and results display are satisfied

### Expected Results

- Flight search is executed, and results are displayed on the 'Search Results' page
- All acceptance criteria for the flight search and results display are satisfied
- Functionality works as specified in the acceptance criteria

---

## Verify a user selects a departure date, THE Flight*Search SHALL enforce that the return date if provided is after the departure date

**Test Case ID:** SCRUM-5-TC-10120
**Category:** Positive
**Automation Readiness:** 🟢 High
**Source Requirement:** desc-1-1

### Description

Test the main functionality described in: WHEN a user selects a departure date, THE Flight*Search SHALL enforce that the return date if provided is after the departure date

### Preconditions

- User is authenticated and has appropriate permissions
- User interface is loaded and accessible

### Test Steps

1. **Action:** Navigate to the flight search page
Enter the following valid search criteria:
- Origin Airport: 'SFO'
- Destination Airport: 'JFK'
- Departure Date: '2023-07-01'
- Return Date: '2023-06-30' before departure date
- Cabin Class: 'Business'
- Number of Passengers: '1'
   **Expected Result:** Search criteria is accepted, but a validation error is displayed for the return date

2. **Action:** Verify the following validation behavior:
- Return date field is highlighted in red
- Error message is shown: 'Return date must be after departure date'
- Search cannot be submitted until valid return date is entered
   **Expected Result:** Validation error is displayed, and search cannot proceed with invalid date combination

3. **Action:**  the return date to a valid date after the departure date e.g., '2023-07-08'
Click the 'Search Flights' button
   **Expected Result:** Search is executed successfully, and results are displayed on the 'Search Results' page

### Expected Results

- Search criteria is accepted, but a validation error is displayed for the return date
- Validation error is displayed, and search cannot proceed with invalid date combination
- Search is executed successfully, and results are displayed on the 'Search Results' page
- Functionality works as specified in the acceptance criteria

---

## Verify a user submits the search form with valid inputs, THE Flight*Search SHALL query available flights and navigate to the Search*Results page

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

1. **Action:** Navigate to the flight search page
Enter the following valid search criteria:
- Origin Airport: 'LHR'
- Destination Airport: 'DXB'
- Departure Date: '2023-08-15'
- Return Date: '2023-08-22'
- Cabin Class: 'First'
- Number of Passengers: '4'
   **Expected Result:** Search criteria is accepted and validated without errors

2. **Action:** Click the 'Search Flights' button
   **Expected Result:** Search is executed, and user is navigated to the 'Search Results' page

3. **Action:** Verify the following on the 'Search Results' page:
- Page title displays the search criteria summary
- Flight results are displayed in a clear and organized manner
- Sorting and filtering options are available
- Pricing information is accurate and up-to-date
   **Expected Result:** All acceptance criteria for the flight search and results display are satisfied

### Expected Results

- Search criteria is accepted and validated without errors
- Search is executed, and user is navigated to the 'Search Results' page
- All acceptance criteria for the flight search and results display are satisfied
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
- User is authenticated and has appropriate permissions
- User interface is loaded and accessible

### Test Steps

1. **Action:** Navigate to the flight search page
Enter valid data in all required fields:
- Origin Airport: 'JFK'
- Destination Airport: 'LAX'
- Departure Date: '2023-06-15'
- Return Date: '2023-06-20' optional
- Cabin Class: 'Economy'
- Number of Passengers: '2'
Click the 'Search Flights' button
   **Expected Result:** Flight search is executed, and results are displayed on the 'Search Results' page

2. **Action:** Verify the search results meet the following acceptance criteria:
- Results are displayed in a clear and organized manner
- All required flight details are shown airline, flight times, duration, stops, etc.
- Sorting and filtering options are available
- Pricing information is accurate and up-to-date
   **Expected Result:** All acceptance criteria for the flight search and results display are satisfied

### Expected Results

- Flight search is executed, and results are displayed on the 'Search Results' page
- All acceptance criteria for the flight search and results display are satisfied
- Functionality works as specified in the acceptance criteria

---

*Generated automatically from Jira acceptance criteria. Focus on positive scenarios and core functionality validation.*
