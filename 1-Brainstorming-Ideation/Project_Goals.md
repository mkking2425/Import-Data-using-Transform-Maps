# Project Goals and Scope

### Main Goal
To automatically import bulk employee data from a spreadsheet into ServiceNow without manual effort and without creating duplicates.

### Objectives
1. To create a Sample Spreadsheet (Sample Spreadsheet.xlsx) with 5 fields: Employee ID, Name, Email, Department, Location.
2. To create a Custom Target Table named u_employee_test to store the final clean data.
3. To create an Import Set Table named u_employee_import as a staging table.
4. To create a Transform Map named "Sample Spreadsheet Import" with Auto Map.
5. To enable Coalesce on Employee ID field to avoid duplicate records.
6. To validate the import by successfully importing 15 sample records.
7. To create Reports and a Dashboard to visualize the imported data.

### Scope of the Project
- In Scope: Data Import, Field Mapping, Duplicate Handling using Coalesce, Data Validation, Reporting.
- Out of Scope: Approval Workflows, Notifications, Advanced Business Rules (will be considered as future enhancements).

### Expected Benefits
- 90% reduction in data entry time.
- 100% duplicate prevention.
- Clean and accurate data for HR and IT teams.
