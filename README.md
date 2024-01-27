# EggNog Analysis (COGs and Base Species)
### Step-by-step analysis
```
0- Upload the databases "banana_emapper.annotations.xlsx" and "rosa_emapper.annotations.xlsx"

1- Delete columns that are not of interest

2- Separate the base species column into another one using the "|" delimiter and delete the column that is not of interest (column with numbers)

3- Change the column names (species and COGs)

4- Remove blank rows and rows with errors from the remaining two columns

5- Split lines with more than one letter into one letter per line using the "Text.ToList([COGs])" command and select the "Expand to new lines" option in the generated custom column

6- Delete the column that is not of interest (column with more than one letter in a line)

7- Dashboard assembly

	7.1- Pie chart to determine the quantity of each COG type in each species, applied a filter excluding the values "S" and "-" as they refer to unidentified functions
 
	7.2- Area chart to analyze from which species the protein function data were extracted and check if it matches the analyzed species, applied a filter excluding the "-" values as they refer to unidentified organisms or functions not identified with any organism in the database
 
	7.3- Card to display the numerical quantity of each COGs classification for the species and quantify how many proteins are encoded by each species, considering the values "S" and "-"
 
	7.4- Bar chart for a better illustration of the numerical quantity on the card and a transparent background to overlay on the card number, applied a filter excluding the values "S" and "-" as they refer to unidentified functions
 
	7.5- Relate data from the sheets in the "Model display" tab so that selecting in one chart generates it in the other charts, enabling a faster comparison between species
 
	7.6- Create a background image
 
		7.6.1- Image created by the artificial intelligence Leonardo.ia with the prompt "Darkness forest seen from above, all trees black"
  
		7.6.2- After downloading the image on the computer, it was inserted into PowerPoint to adjust the size according to the Power BI dashboard
  
	7.7- Adjust all charts with a transparent background, legend coloring for visibility, and change the coloring of certain charts
 ```
### Result
#### Dashboard without any selection
![image](https://github.com/Tutugb/powerBI/assets/125391314/3cf9ba11-7eca-4eb5-b9bf-74e8f241ffc3)
#### Dashboard with selection
![image](https://github.com/Tutugb/powerBI/assets/125391314/b8853639-1365-473b-9cb7-9aeccf057cd3)

# Sales and Profit Analysis 
```
0. Upload the "Online Retail.xlsx" database
1. Data processing

	2. Delete columns that are not of interest

	3. Rename columns

	4. Multiply "quantity sold" and "price" creating "sold"

	5. Split the price column by delimiter "-" to remove negative values, which are incorrect since there is no negative price

	6. Replace "null" values with 0

7. Dashboard assembly

	8. First bar chart with line where the common x-axis is the date with only month and year, but the y-values for the bars are the quantity sold and the line values are the cumulative value (column "sold")

	9. Second bar chart with line where the common x-axis is the date with only month and year, but the y-values for the bars are the quantity sold and the line values are the product prices

	10. First pie chart with the cities that made sales, thus analyzing which sold more

	11. Second chart of the products sold, analyzing which product was sold the most

	12. First card with the value of the sum of the cumulative value with the sales (column "sold")

	13. Second card with the value of the sum of the quantity sold of the products in general

 	14. First filter, select the year to analyze

 	15. Second filter, select the month to analyze

 	16. Third filter, select the city to analyze

 	17. Fourth filter, select the product to analyze

	18. Background done in PowerPoint
```
### Result 
#### Dashboard without any selection
![image](https://github.com/Tutugb/powerBI/assets/125391314/a7db8521-6786-4ddb-a5f8-ff83929c6e44)
#### Dashboard with selection
![image](https://github.com/Tutugb/powerBI/assets/125391314/350056c7-024c-4f04-9be3-d15a31e7bedd)
