# GenAI Manual Test Engineer – Demo QA Portfolio

This repository is my hands‑on portfolio for a **GenAI Manual Test Engineer** role.  
It demonstrates end‑to‑end manual testing on a realistic web application, using **AI as an accelerator** while applying solid QA fundamentals.

## Target Application

- **Application:** [demoqa.com](https://demoqa.com)  
- **Focus Area:** Forms (Practice Form), Alerts, and basic UI elements.  
- **Why this app:** It simulates common internal tools with forms, validations, modals, and alerts, making it suitable to practice functional, negative, and exploratory testing.

## Tools & Environment

- **Browser:** Chrome (latest)
- **Issue & Defect Tracking:** Jira (Bug tracking project)
- **Test Management Concept:** Jira + Zephyr style (test cases linked to requirements/bugs, test cycles, traceability)
- **API Testing:** Postman (against [reqres.in](https://reqres.in))
- **Database Validation:** Online SQL sandbox (e.g., sqliteonline.com)
- **Version Control & Documentation:** GitHub (this repo)
- **AI Assistance:** Used to help generate and refine requirements, test scenarios, test cases, SQL queries, and reports (all outputs reviewed and adapted manually)

## Repository Structure

- `notes/` – Environment setup and application overview.
- `requirements/` – Functional and non‑functional requirements for the Practice Form.
- `test-design/` – Test scenarios and detailed manual test cases (CSV/Markdown).
- `execution/` – Test execution results and test summary report.
- `defects/` – Defect templates and summary of logged bugs (actual defects tracked in Jira).
- `exploratory/` – Exploratory testing charters and session reports.
- `api-tests/` – API test scenarios and Postman collection.
- `sql/` – Database schema, sample data, and validation queries.
- `genai-qa/` – Risk matrix, AI prompts library, and GenAI‑focused QA notes.
- `projects/practice-form-stlc/` – End‑to‑end mini‑project applying the full STLC on the Practice Form.

## What This Project Demonstrates

### Requirement Analysis

- Analyzed the Practice Form requirements to identify:
  - Confirmed functional rules, including required and optional fields, validations, date restrictions, submission behavior, usability, performance, and accessibility.
  - Missing requirements and clarification questions about field limits, special characters, error messages, confirmation-modal content, file uploads, dropdowns, accessibility standards, mobile support, and data persistence.
  - Key risks related to user frustration, invalid data, accessibility, performance, future dates, file uploads, lost data, and unclear confirmation details.
- Used this analysis as the foundation for test scenarios, test cases, and risk assessment.

### 1. End‑to‑End STLC on a Web Feature

- Analyzed requirements for the **Practice Form** feature.
- Designed **test scenarios** and **detailed manual test cases** (positive, negative, edge).
- Executed tests, logged defects in **Jira**, and performed regression on critical paths.
- Produced a **test summary report** with pass/fail counts, open defects by severity, and key risks.

### 2. Risk‑Based Testing

- Built a simple **risk matrix** (likelihood × impact) for form areas (email, mobile, required fields, date of birth, file upload, error messages).
- Prioritized test design and execution to cover **high‑risk areas first**, especially under time constraints.

### 3. AI‑Assisted Test Design (GenAI Angle)

- Used AI to:
  - Draft requirements and acceptance criteria.
  - Generate initial test scenarios and test cases.
  - Identify coverage gaps and suggest additional edge cases.
  - Help design SQL validation queries and draft test reports.
- Applied QA judgment to:
  - Review, refine, and prioritize AI output.
  - Remove duplicates and clarify steps.
  - Ensure traceability to requirements and real‑world risk.

This shows I can use GenAI as a **productivity multiplier** without compromising quality or critical thinking.

### 4. API & Database Validation

- Designed API test scenarios for a REST API (reqres.in) using **Postman**.
- Validated status codes, response bodies, and error handling.
- Created a simple database schema (`users`, `orders`) and practiced **SQL queries** (SELECT, JOIN, aggregation) to verify data integrity, simulating backend validation for UI/API actions.

### 5. Exploratory Testing

- Ran time‑boxed exploratory sessions (e.g., on the Alerts module) with clear charters.
- Documented coverage, findings, risks, and recommendations in concise session reports.
- Logged defects in Jira for issues discovered during exploration.

### 6. Alignment with Jira + Zephyr Practices

- Defects are logged in **Jira** with clear steps, expected vs actual results, severity/priority, environment, and attachments.
- Test scenarios and cases in this repo reflect how they would be managed in a **Jira + Zephyr** setup:
  - Test cases linked to requirements/user stories.
  - Test cycles per sprint/release.
  - Failed tests linked to bug issues.
  - Traceability from requirement → test → defect.

This repo is a portfolio artifact; in a real team, the same test cases would live in Zephyr inside Jira.

## How to Navigate This Repo

Start here if you are:

- **A recruiter or hiring manager:**  
  - `projects/practice-form-stlc/` – Full STLC on one feature.  
  - `execution/test-summary-report.md` – Quick view of results and defects.  
  - `genai-qa/` – How I used AI in QA.

- **A technical interviewer:**  
  - `requirements/practice-form-requirements.md` – Requirements quality and clarity.  
  - `test-design/test-cases-practice-form.csv` – Test design skills.  
  - `api-tests/` and `sql/` – API and data validation basics.  
  - `exploratory/` – Exploratory testing approach.

## Notes on AI Usage

- AI was used as an **assistant**, not as a replacement for QA thinking.
- All AI‑generated content (requirements, test cases, queries, reports) was:
  - Reviewed for correctness and completeness.
  - Adapted to match realistic QA standards.
  - Prioritized based on risk and business impact.
