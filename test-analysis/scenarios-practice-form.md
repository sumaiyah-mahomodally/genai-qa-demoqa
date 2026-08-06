| Scenario ID | Scenario Description                                                                 | Covered Requirements      |
|-------------|--------------------------------------------------------------------------------------|---------------------------|
| TS01        | Verify that all required form fields (First Name, Last Name, Email, Mobile, Gender, Date of Birth, Address, City, State, Zip Code, Country) are present and visible. | FR1                       |
| TS02        | Validate that the Email field accepts only valid email formats and rejects invalid ones. | FR2                       |
| TS03        | Validate that the Mobile Number field accepts exactly 10 digits and rejects non-numeric or incorrect length inputs. | FR2                       |
| TS04        | Validate that Date of Birth cannot be set to a future date.                          | FR2                       |
| TS05        | Validate that Zip Code field accepts only numeric input.                             | FR2                       |
| TS06        | Attempt submission with missing required fields and verify error messages are displayed near invalid fields. | FR2, FR3                  |
| TS07        | Submit the form with all valid inputs and verify that a confirmation modal appears with submitted data summary. | FR3                       |
| TS08        | Verify optional fields (Hobbies checkboxes, Profile Picture upload) can be left empty without blocking submission. | FR1                       |
| TS09        | Verify that all labels are clearly visible and correctly associated with their respective fields. | FR4                       |
| TS10        | Verify form usability across supported desktop browsers (Chrome, Firefox, Edge).     | FR4                       |
| TS11        | Verify that the form page loads within 3 seconds on a standard broadband connection. | NFR1                      |
| TS12        | Verify that all form fields have proper labels for screen readers (basic accessibility check). | NFR2                      |
| TS13        | Attempt submission with multiple invalid inputs (e.g., invalid email + short mobile number) and verify multiple error messages are displayed correctly. | FR2, FR3                  |
| TS14        | Verify form behavior after successful submission (form cleared or remains filled as per design). | FR3                       |
| TS15        | Verify that dropdowns (State, Country) display correct options and allow valid selection. | FR1                       |
