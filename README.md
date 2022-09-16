# echoxladdin
Excel VBA addin to work with Labcyte Echo transfer reports and pick lists/plate maps


## Modules:
  - Create a pick list
  - Plate Maps
    - Inspect Plate Maps
    - Create a new plate map
  - Process Transfer File
  
## How to use it:

All modules require the source plate maps to be standardised. For an example, create a new plate map.

### Create a pick list

- A new workbook is created with "Input" and "Pick List" worksheets.

- On the "Input" sheet, enter the IDs of samples you want to plate out.

- When you click on the "Create Picklist" button, a new dialog will open.

- On this dialog, select the directory in which your plate maps are stored,
  select which (or all) plate maps you want to search. You can also
  restrict the source concentration.

- After you've pressed "Start", the script will open all specified files
  and search for your sample IDs. The screen might flicker a bit.

- Once done, your pick list will be on the "Pick List" worksheet. Note that
  ALL instances of the specified samples will be listed, so you will have to
  manually curate.

### Plate Maps

#### Inspect Plate Maps

- A simple file browser that displays all .xlsx files in a specified
  directory.

#### Create a new plate map

- Creates a workbook with the required columns for a standardised plate
  map.

### Process Transfer File

- User gets prompted to select a  Labcyte Echo transfer report in .csv format.
- This module extracts Destination Plate names, sample IDs, locations, and final assay concentrations (as calculated by the Echo).
