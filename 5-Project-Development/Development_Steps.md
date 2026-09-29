# Development Steps - Import Data using Transform Maps

### Step 1: Prepare Sample Spreadsheet.xlsx
- Create Excel file with 5 columns: Employee ID, Name, Email, Department, Location
- Add 15 sample records (e.g., EMP001, John Doe...)

### Step 2: Create Target Table (u_employee_test)
- Navigate: System Definition -> Tables -> New
- Label: Employee Test, Name: u_employee_test
- Add 5 fields: u_employee_id (String, Coalesce), u_name (String), u_email (Email), u_department (String), u_location (String)

### Step 3: Load Data using Import Sets
- Navigate: System Import Sets -> Load Data
- Import Set Table: Create new -> u_employee_import
- Upload Sample Spreadsheet.xlsx
- Click "Load"

### Step 4: Create Transform Map (Main Step)
- Navigate: System Import Sets -> Transform Maps -> New
- Name: Sample Spreadsheet Import
- Source Table: u_employee_import
- Target Table: u_employee_test
- Click Save -> Click "Auto Map Matching Fields" -> Click "Transform"
- Check Coalesce is enabled for Employee ID field

### Step 5: Verify Data
- Navigate: u_employee_test table -> Check 15 records imported successfully
- Test Duplicate: Upload same sheet again -> Should show 0 inserted, 15 updated (No duplicate)
