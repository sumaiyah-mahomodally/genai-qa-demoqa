# Requirement Analysis — Practice Form (demoqa.com)

---

**Objective:** Critically analyze the practice form requirements, identify functional rules, missing questions, risks, and clarifications.  

**Task:** Review the provided requirements and raise at least 10 clarification points.  

**Deliverable:** Structured requirement analysis note.  

---

## 1. Functional Rules

> What the system must do — confirmed from the requirement

| # | Rule |
| :-: | :--- |
| 1 | **Required Fields** — First Name, Last Name, Email, Mobile Number, Gender, Date of Birth, Address, City, State, Zip Code, Country must be completed before submission |
| 2 | **Optional Fields** — Hobbies (checkboxes) and Profile Picture (file upload) are optional |
| 3 | **Format Validation** — Email must follow valid format; Mobile must be exactly 10 digits numeric; Zip Code must be numeric |
| 4 | **Date Validation** — Date of Birth cannot be a future date |
| 5 | **Submission Success** — Confirmation modal appears with submitted data summary |
| 6 | **Submission Failure** — Error messages displayed near invalid fields; form not submitted |
| 7 | **Usability** — Labels must be visible and associated with fields; form usable on Chrome, Firefox, Edge |
| 8 | **Performance** — Page must load within 3 seconds on broadband |
| 9 | **Accessibility** — Fields must have proper labels for screen readers |

---

## 2. Missing Questions

> Gaps the requirement did not address — written as questions a QA intern should raise

| # | Question |
| :-: | :--- |
| 1 | **Field Length Limits** — What are the min/max character lengths for First Name, Last Name, Address, City, etc.? |
| 2 | **Special Characters** — Are hyphens, apostrophes, or spaces allowed in names and addresses? |
| 3 | **Error Message Texts** — What exact wording should appear for each validation error? |
| 4 | **Confirmation Modal Content** — Should it display all submitted fields or only key details? |
| 5 | **Form Reset Behavior** — After successful submission, should the form clear or remain filled? |
| 6 | **File Upload Constraints** — What file types and sizes are allowed for profile picture uploads? |
| 7 | **Dropdown Options** — Are State and Country dropdowns predefined lists, and how are they maintained? |
| 8 | **Accessibility Standards** — Should the form meet WCAG 2.1 compliance or only basic label association? |
| 9 | **Mobile Responsiveness** — Is the form required to work on mobile devices or only desktop browsers? |
| 10 | **Data Persistence** — If submission fails, should entered values remain or be cleared? |

---

## 3. Key Risks

> What could go wrong if these gaps are not resolved

| # | Risk |
| :-: | :--- |
| 1 | **User Frustration** — Vague error messages may confuse users |
| 2 | **Invalid Data Entry** — Missing field length rules may allow malicious or nonsensical input |
| 3 | **Accessibility Failures** — Non-compliant labels may exclude users with disabilities |
| 4 | **Performance Complaints** — Slow page load may cause users to abandon the form |
| 5 | **Future DOB Exploit** — Without strict validation, users could bypass age restrictions |
| 6 | **File Upload Issues** — Undefined constraints may cause crashes or security vulnerabilities |
| 7 | **Lost Data** — If failed submissions clear fields, users may abandon the process |
| 8 | **Inconsistent Confirmation** — Ambiguous modal content may mislead users about what was submitted |

---

## 4. Clarification Questions

> 10 questions to raise before development starts

| # | Question | Category |
| :-: | :--- | :---: |
| 1 | What exact error messages should appear for each invalid field? | Validation |
| 2 | What are the min/max character lengths for text fields (names, address, city)? | Validation |
| 3 | Are special characters allowed in names and addresses? | Validation |
| 4 | Should the confirmation modal display all submitted data or only key fields? | UX |
| 5 | After successful submission, should the form clear or remain filled? | UX |
| 6 | What file types and sizes are allowed for profile picture uploads? | Validation |
| 7 | Are State and Country dropdowns static lists or dynamically updated? | Business Rule |
| 8 | Should the form meet WCAG 2.1 accessibility standards? | Compliance |
| 9 | Is mobile responsiveness required, or only desktop browsers? | Non-Functional |
| 10 | Should failed submissions preserve entered values for user convenience? | UX |

---

## 5. Summary

> Even a simple form can hide gaps that affect usability, compliance, and security.  
>
> - **Functional rules** define expected behaviors  
> - **Missing questions** highlight unclear or incomplete details  
> - **Key risks** show potential failures if gaps are ignored  
> - **Clarification questions** ensure alignment before development begins  

---
