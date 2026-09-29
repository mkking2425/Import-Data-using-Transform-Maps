# Architecture Diagram

### Components Used in ServiceNow:
1.  **System Import Sets -> Load Data:** Excel file upload pannarathukku.
2.  **System Import Sets -> Import Set Table (u_employee_import):** Temporary data store pannarathukku (Staging).
3.  **System Import Sets -> Transform Maps:** Staging table la irunthu Target table ku map pannarathukku. Itha thaan heart of project.
4.  **Target Table (u_employee_test):** Final data store pannarathukku.
5.  **Reporting & Dashboard:** Data visualize pannanum.

### Architecture Flow:
User (Admin) uploads Sample Spreadsheet.xlsx -> ServiceNow creates Import Set -> Data goes to u_employee_import -> User clicks "Transform" -> Transform Map (Sample Spreadsheet Import) runs with Coalesce logic on Employee ID -> If Employee ID exists, update, else insert -> Data saved in u_employee_test.

### Transform Map Details:
- Name: Sample Spreadsheet Import
- Source Table: u_employee_import
- Target Table: u_employee_test
- Field Maps: 5 fields auto-mapped
- Coalesce: True for u_employee_id
