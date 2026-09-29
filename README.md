# Import Data using Transform Maps - ServiceNow Project

**Project Domain:** ServiceNow Development
**Project Title:** Import Data using Transform Maps with Coalesce

### Project Description
This project automates bulk employee data import from Excel (Sample Spreadsheet.xlsx) to ServiceNow Target Table (u_employee_test) using Import Sets and Transform Maps. It solves the manual data entry problem for HR teams and prevents duplicate records using Coalesce on Employee ID.

### Key Features Implemented
- Automated bulk import of 15+ records in 15 seconds (vs 1 hour manually)
- Duplicate prevention - 100% using Coalesce on Employee ID
- Auto Map for 5 fields: Employee ID, Name, Email, Department, Location
- Staging Table (u_employee_import) and Target Table (u_employee_test)
- Transform Map: "Sample Spreadsheet Import"
- Reports and Dashboard by Department/Location

### Architecture Flow
Excel -> Load Data -> Staging Table (u_employee_import) -> Transform Map (with Coalesce) -> Target Table (u_employee_test) -> Reports

### Project Phases Completed
- Phase 1: Brainstorming & Ideation - DONE
- Phase 2: Requirement Analysis - DONE
- Phase 3: Project Design - DONE
- Phase 4: Project Planning - DONE
- Phase 5: Project Development - DONE
- Phase 6: Functional & Performance Testing - DONE
- Phase 7: Demo Video and Report - DONE

### Results
- Performance: 99% time saved
- Accuracy: 100% data accuracy
- Duplicates: 0 duplicates

**This project demonstrates ServiceNow best practices for data import.**
