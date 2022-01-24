##Info about the project and dataset:
1.The problem description states to analyze how a particular organization performed for its volume in Q2.
2.The data includes two sheets, one for Volume(CLID, Date, Vol) and another for Geographical Region(CLID, GEOID).

Data Cleaning
1. To start with cleaning process, first copied the original data into two new sheets - Volume_data and Geo_data and transformed the data into data tables.
2. Removed the blank cells in Volume_data, and filled it with corresponding CLID.
        1. Ctrl + Space.
        2. Alt H F D S K.
        3. In cell A3 : =A2.
        4. Hold Ctrl and Enter.
4. Reformatted the dates and values from text in Volume_data sheet.
5. Checked for Dulicates value Using shortcut Alt A M.
6. Extracted the CLID in Geo_Data sheet Using =MID() Function so that it matches the same field in Volume_data sheet.
7. Added new fields RegionID and RegionName in Volume_data sheet and GeoName in Geo_Data Sheet using INDEX/MATCH() and VLOOKUP() functions.
8. Checked the consistency of data using SUMIFS() function.
9. Extracted Quarters from Dates field using two separate methods:
        1.="Q"&ROUNDUP(MONTH([@Date])/3,0)&" "&YEAR([@Date])
        2.Using the VLOOKUP() function with the help of Dates table.

Excel file after Data Cleaning Process
1. ![image](https://user-images.githubusercontent.com/97116496/150756571-32ef9213-24a9-4a53-9fee-b8d2e1a94df4.png)
2. ![image](https://user-images.githubusercontent.com/97116496/150756625-ab2e6c8e-7b53-40f4-848b-cfc3fe58e391.png)



Dataset
This dataset is obtained from Matt Brattin's Github Repository of Excel-for-Analytics : https://github.com/mattbrattin/Excel-for-Analytics


