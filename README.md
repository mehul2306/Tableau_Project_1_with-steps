# Tableau_Project_1_with-steps
 Basic Graphs and Charts in Tableau
The objective of this exercise is to use learn how to create basic charts in Tableau and to know when to use a particular chart, how using a chart makes the understanding of underlying data easy. The data is for purchase orders from a store between Dec 2014 and June 2015.

Step 1:
Download the dataset from eLearning.
Import the dataset in Tableau. To import the data, you need to click on Microsoft Excel on the home screen of Tableau and select the file to be imported.
Under sheets you will find the names of two sheets. If you look at your dataset in excel, you will find those two sheets there. Now you can choose the sheet on which you want to create visualization. You can choose both the sheets too. In the case of selecting both the sheets, a join will be created based on the columns in the sheets.
For this exercise, we will choose only ‘Orders’ sheet. To select this sheet, drag it to the area labelled with text “Drag sheets here”.
 

Click on Sheet 1 in bottom left corner.
 
This will create a new sheet for you to work upon.
There are two columns in the data set – Product_Category and Product_Sub-Category. Here we would like to visualize which product sub category has the highest number of sales under a particular product category. The best way to visualize this would be a bar chart.
Drag product category and product sub category to rows and number of records to columns. The default level of aggregation for number of records is SUM and hence you will see the word SUM when you drag it to columns.
 

After dragging number of records to column, you will see that a horizontal bar chart is prepared for you. If you like to change the axis you need to click on   in the tool bar. It will change the bar chart from horizontal to vertical or from vertical to horizontal. For our exercise, we will go with horizontal bar chart.
If you look at the bar chart you will notice that the bars are not in order and this makes the bar chart less aesthetic. To make a bar chart visually appealing, we must sort the bar chart either ascending or descending, with a few exceptions like when we are creating bar charts for visualizing temperature on each day of a week, it is better to have the chart sorted based on the days and not sorted based on values of temperature.
To sort our bar chart, hover your mouse just above the bars of the first product sub category. You will find an icon for sorting. Click on that icon to sort the bars.
 
Alternatively, you can click the icon    in the tool bar to sort the data in descending order.
Now, look at your bars and try to figure out the number of products sold in each sub category. Is it little bit cumbersome to figure out the value for each product sub category. We will try to get rid of this and make our visualization more informative at first glance.
Drag Number of records to Label under Marks.
 
This will make the number of sales under each product sub category appear at the tip of the bar.
Also, the chart will look good if we make the colour of the chart vary according to the number of records. Drag Number of records to Color under Marks. The color of the bars will change, most number of product sold being the darkest and least number of products sold being the lightest in color.  You can see a legend for the same in the right upper corner.
Click on the down arrow mark in the legend and then select Edit colors. Select Red-Gold from the drop down and click Apply and then OK.
Give the sheet a name “No of Product Sold Based on Sub Category”
Questions:
1.	Paste the screenshot of your sheet.
 

2.	How many envelopes have been sold during the given period? (No need of screenshot)
Answer : 10480000
3.	List the product sub category and the number of units sold under each product category having the highest number of units sold? (No need of screenshot)
Answer :
Product Sub-category  – Furnishing > Bookcases, Chairs & Chairmats, Office Furnishings, Tables
Office Supplies > Appliances, Binders & Binders Acc; Envelopes, Labels, Paper, Pen& Art Supplies; Rubber Band, Scissor, Rulers & Trimmers; Storage & Organisation
Technology >Computer Peripherals, Copiers & Fax Machines, Office Machines, Telephones &  Communication
Highest Unit Sold : Furnishing – Chairs & Chairmats : 261,073K
Office Supplies - Binders & Binders Acc : 185,928K
       Technology - Office Machines – 318,170K

4.	In office supplies product category, which sub category ranked third in terms of sell? (No need of screenshot)
Answer : Applianes : 82,201K

Step 2:
Click on the new worksheet icon to create a new worksheet.  
In this sheet we will try to visualize the sales data and profit earned weekly.
Drag Order date to column. Right click on it and select “Week Number”. Drag Product Category to rows. Now drag “Sales” to rows. You will find that a time series has been plotted. Tableau decides on its own which graph to use for a particular kind of data. We can override this by clicking on “Show Me” and selecting our desired chart type.  In the Show Me section, Tableau will show you all the charts which are compatible with the data.
For this step we will select the bar chart.
Now drag profit to rows. We need to convert the chart type of Profit. Click on SUM(Profit) in Marks and select the Area chart.
 
You will see the chart below for each category.
 
Now, inside the chart, right click on Profit under Furniture category and select Dual Axis. Now you can see how the profit and sales are overlapped on each other giving us a view that tells both week wise sales and profit in that particular week. But there is still a problem. Look at the axes. The axis on the left is for sales and the axis on the right is for profit. Both have different intervals which is making the visualization misleading. 
Now, right click on the axis of profit and select synchronize axis. This will synchronize both the axis to get the meaningful information.
Give your sheet a name “Weekly Sales and Profit”.
5.	Paste the screenshot of your visualization.
 
6.	In which week, does the profit highest for Furnitures and how much? (No Screenshot needed)
Answer : Profit - May 3,2015 & 11,666K
7.	What is the sales in that week for Furnitures? (No Screenshot needed)
Answer : 39902K
8.	What is the ratio of profit to sales in that week for Furnitures? (No Screenshot needed)
Answer :- 5833 : 19951
Step 3:
Create a new sheet. 
Drag customer_segment to rows and number of records to column. Click on Show Me and select Packed Bubble. You can see four bubbles created on the sheet. The size of each bubble shows the number of customer in that segment.
Now remove the customer_segment from Color. 
Drag profit into color. Then, drag profit and number of records to Labels.
Give a name to your sheet “Customer Segment -Wise Profit”.
9.	Paste the screenshot of your sheet.
 

10.	Which customer segment gives the maximum profit and how much. (No screenshot needed.)
Answer : Small Business 65,305K
11.	There is something peculiar which we can notice from this bubble chart regarding size of customer base and profit. What is that thing? (No screenshot needed.)
Answer : The peculiar thing about this bubble chart is that the small business is having the lowest no of records still has the highest profit. And Corporate has the highest number of records & not much profit.
Step 4:
Create a new sheet.
Drag Region to rows and Number of records to column. Click on Show Me and select Treemaps.
Right click on SUM(Number of Records) which you have put into Lable, and not the one into color.
 
Select “Quick Table Calculation” from the drop down and then select “Percentage of Total”. Do the same for SUM(Profit). You will see the labels inside your char will get converted into percentage. 
Give a name to your sheet “Region-wise Sales and Profit”.
12.	Paste the screenshot of your sheet.
 

13.	Which region is in loss and by what percentage? (No screenshot needed.)
Answer : South by -6.44%

14.	Which region is in maximum profit? (No screenshot needed.)
Answer : East by 38.06%

Step 5:
Create a new sheet.
Drag Country to the sheet. You will get the map of US. Then drag State to the sheet. You will find all the states labelled by a dot on the map.  After this drag profit to color and label. You will see that all the states will get color coded according to the profit made by that state.
Now right click on SUM(Profit) and select Format…
Click on the Pane panel and then down arrow in the Font textbox. Select Tableau Bold as the font make the font size 10. 
Give a name to your sheet “State-Wise Profit”
15.	Paste the screenshot of your sheet.
 


16.	Which state is having the highest profit? (No screenshot needed.)
Answer :  California
17.	What is the profit of Nebraska? Place your pointer on Nebraska so that the tool tip is visible and paste the screenshot.
Answer : 4676 
 











