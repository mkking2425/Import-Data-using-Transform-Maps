# User Stories

**User Story 1: As an HR Admin, I want to upload bulk employee data**
- As a: HR Admin
- I want to: Upload Excel file with 15+ employee records
- So that: I can avoid manual typing and save time
- Acceptance Criteria: System should accept .xlsx file

**User Story 2: As a System, I want to prevent duplicate records**
- As a: System
- I want to: Check if Employee ID already exists
- So that: Duplicate employees are not created
- Acceptance Criteria: If Employee ID exists, update record, else insert new record. Coalesce = True.

**User Story 3: As an IT Manager, I want to see reports**
- As a: IT Manager
- I want to: View report of employees by Department and Location
- So that: I can track HR data easily
- Acceptance Criteria: Dashboard should show count by Department
