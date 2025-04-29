# Employee Data Consolidation

This script consolidates employee data from multiple sources, including office addresses, employee roles, and emergency contacts into a unified Dataframe.

## Input Files

Place all datasets in the 'datasets/' directory:

- `office_addresses.csv`- Contains office location data.
- `employee_information.xlsx`- Contains employee addresses and emergency contact details (sheet: `emergency_contacts`).
- `employee_roles.json`- Contains roles indexed by `employee_id`.

## How It Works

1. Reads in office, address, emergency contact, and role data.
2. Merges the datasets based on employee ID and country.
3. Fills in missing office details with `"Remote"`.
4. Outputs a clean DataFrame with selected columns and `employee_id` as the index.

## Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
