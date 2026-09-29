# Data Flow Diagram

Excel (Sample Spreadsheet.xlsx) 
   |
   v
[System Import Sets] -> [Load Data] 
   |
   v
Staging Table (u_employee_import) - 15 records here
   |
   v
Transform Map (Sample Spreadsheet Import) - Logic applied here (Coalesce check)
   |
   v
Target Table (u_employee_test) - Final clean data
   |
   v
Reports & Dashboard
