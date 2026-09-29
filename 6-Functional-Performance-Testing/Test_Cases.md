# Test Cases - Import Data using Transform Maps

### Test Case 1: Successful Import of 15 Records
- Objective: Check if all 15 records from Excel are imported to target table
- Steps: Load Data -> Select u_employee_import -> Upload Sample Spreadsheet.xlsx -> Transform
- Expected Result: 15 records inserted in u_employee_test table
- Actual Result: 15 records inserted - PASS

### Test Case 2: Duplicate Prevention using Coalesce
- Objective: Ensure duplicate Employee IDs are not created
- Steps: Upload same Excel file again and Transform
- Expected Result: 0 inserted, 15 updated. Total count remains 15.
- Actual Result: 0 inserted, 15 updated - PASS - No duplicates created

### Test Case 3: Field Mapping Validation
- Objective: Check if all 5 fields are mapped correctly
- Steps: Check target table records vs Excel data
- Expected Result: Employee ID, Name, Email, Department, Location matches exactly
- Actual Result: All fields matched - PASS

### Test Case 4: Invalid Data Handling
- Objective: Check behavior with empty Employee ID
- Steps: Upload Excel with empty Employee ID
- Expected Result: Record should be ignored or error shown
- Actual Result: Error handled - PASS

### Test Case 5: Report Validation
- Objective: Check if reports show correct data
- Steps: Open Reports -> Department wise count
- Expected Result: Report shows correct count
- Actual Result: Report shows correct count - PASS
