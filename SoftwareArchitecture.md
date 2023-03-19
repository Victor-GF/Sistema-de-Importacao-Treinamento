# Software Architecture
We have the following characteristics for the software:

## Responsible
The program needs to deal with improper formatting in the spreadsheet, making changes like:

- Removing incorrect spacing and special characters 
- Capitalizing the initial letters of the name
- Change the CPF to the format 123.456.789-00

And it must also alert the user in cases of incorrect formatting that cannot be corriged, for example:

- Null values
- Letters in number fields only and vice versa


