The Dataset: 
An e-commerce order list with customer details, product info, and fulfillment status.

The Problems I Found:
Inconsistent Product/Brand Names: e.g., Nike, Nike Inc., Nike UK; MagisTA SHoes, FootBALL SHIRt.
Combined "Location" Column: e.g., London UK, Tampa USA needed splitting into City and Country.
Combined "Contact" Column: Bill_Smith needed splitting into First and Last name.
Missing Data: Missing Brand, Product, Contact, and Fulfillment values.
Inconsistent Fulfillment Format: Stored as integers (0, 30, 100) instead of decimals or percentages (0, 0.3, 1.0).
Inconsistent Price Format: Used commas as decimals (e.g., 122,79).

My Cleaning Process:
Standardization: Created consistent brand and product names (e.g., all Nike, Football Shoes).
Text-to-Columns: Used _ and space delimiters to split Contact and Location into new columns.
Handling Missing Data: Filled blanks with NA to be explicit.
Data Transformation: Converted Fulfillment from integers to decimals by dividing by 100.
Number Formatting: Replaced commas with periods in the Price column to convert European number format to a standard numeric format.

The Outcome: 
A perfectly structured dataset ready for customer analysis, inventory management, and sales reporting.
