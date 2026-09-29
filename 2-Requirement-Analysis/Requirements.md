# Requirement Analysis - Import Data using Transform Maps

### 1. Stakeholders
- HR Team: Data kudupanga (Excel owner)
- ServiceNow Admin/Developer (We): Import pannuvom
- IT Manager: Final reports paarpanga

### 2. Functional Requirements
- FR1: System should allow uploading of Excel file (.xlsx)
- FR2: System should have a Staging Table (u_employee_import) to hold temporary data
- FR3: System should have a Target Table (u_employee_test) to hold final clean data
- FR4: Transform Map should auto-map 5 fields: Employee ID, Name, Email, Department, Location
- FR5: Coalesce should be enabled on Employee ID to prevent duplicates
- FR6: Should be able to import 15+ records at a time

### 3. Non-Functional Requirements
- NFR1: Performance - 1000 records should be imported in less than 2 minutes
- NFR2: Accuracy - 100% data accuracy, no manual error
- NFR3: Usability - No coding, admin can do it easily

### 4. Tables & Fields Design

**Target Table: u_employee_test**
| Field Label | Field Name | Type | Coalesce |
| --- | --- | --- | --- |
| Employee ID | u_employee_id | String | Yes |
| Name | u_name | String | No |
| Email | u_email | Email | No |
| Department | u_department | String | No |
| Location | u_location | String | No |

**Staging Table: u_employee_import**
- Same 5 fields as above (Auto created by import)

**Transform Map: Sample Spreadsheet Import**
- Source: u_employee_import
- Target: u_employee_test
- Mapping: Auto Map
