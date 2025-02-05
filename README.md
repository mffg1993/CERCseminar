# Seminar Assignment Script

## Overview
This script automates the assignment of seminar dates to members while ensuring that:
- Members from the same group do not appear consecutively.
- Assignments respect a minimum gap from previous seminar dates.
- Members are not assigned more than once.

The script reads data from an **Excel file** containing:
1. A list of members, their group allocations, and their previous seminar dates.
2. A schedule with available seminar dates (some of which may already be assigned).

The script then fills in unassigned dates while considering the constraints and saves the updated schedule back to the Excel file.

## Requirements
This script requires the following Python packages:
- `pandas`
- `openpyxl`

To install the dependencies, run:
```sh
pip install pandas openpyxl
```

## Usage
1. **Prepare the Input Excel File**:
   - The file should have two sheets:
     - **Sheet1**: Contains members, their group allocations, and their previous seminar dates.
     - **Sheet2**: Contains seminar dates with a "Person" column (some slots may be empty).

2. **Run the Script**:
   - Modify the `input_file` variable in the script to point to your Excel file.
   - Execute the script:
   ```sh
   python assign_dates_by_group.py
   ```

3. **Check the Output**:
   - The script generates an updated Excel file with assigned seminar dates.
   - The output file is saved as `updated_assignments.xlsx`.

## File Structure
```
📂 Project Directory
├── assign_dates_by_group.py  # Main script
├── Book1.xlsx                # Input Excel file
├── updated_assignments.xlsx  # Output Excel file
└── README.md                 # Documentation (this file)
```

## Acknowledgments
- **Code authored by ChatGPT** based on user requirements.
- The script logic was refined through multiple iterations based on user feedback.
- Contributions and improvements are welcome!

