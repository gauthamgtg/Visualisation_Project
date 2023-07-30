<h1 align="center">Zomato Visualisation Project</h1>

<p align="center"><i>Data Cleaning using Tableau Prep Builder</i></p>

<h2>Data Flow:</h2>

![Zomato data cleaning](https://github.com/gauthamgtg/Visualisation_Project/assets/128295307/105d2f74-0ca9-4200-90d5-5b38bbf1bceb)


##  Issues with Data:

<h3 align="center">Restaurant Names</h3>

Example - #45, #Urban Cafí©, {Niche} - Cafe & Bar

* Used REGEXP_REPLACE to remove symbols like #,{,},@ present in the Restaurant Names. 
* Manually modified one entry 'Ohana to Ohana
Fixed null in Cuisines - 
* Found cuisine null for 6 restaurants.
* On searching the restaurant name in Google, Found the cuisine was American for those 6 restaurants. Modified Null with American.

_**### A single restaurant has multiple cuisines**_

Example: Jungle Jamboree -  Continental, Chinese, Thai, Mughlai, North Indian
* Split the cuisine column by comma and unpivot the columns.
* Transformed data to accommodate all the cuisines present in the restaurant
* Each row has a unique restaurant and cuisine combo.

**### Changed column names appropriately**

**### Exported the output as CSV for universal usage**

Data Visualisation using Tableau:
