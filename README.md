# PowerBI_Reimbursed_Cost_Analysis
I have build up a dashboard where we can find Reimbursed cost project wise and slicer. 

Modification that I have done on this file, given below: 


Import the data and open the Power Query
The expense type column has some spelling and punctuation errors, correct them
Project names are not uniform, make it uniform.
The Currency column has some missing values, based on the amount, create a new custom column.
Condition: amount >= 1000, = INR; amount < 1000, = USD; else = EURO
Formula: (if [Currency] = null and [Amount] >= 1000 then "INR" else if [Currency] = null and [Amount] < 1000 then "USD" else [Currency] )
Normalize the amount column into INR based on the currency column.
Created a measure to calculate the sum of reimbursed amount in INR.
Used the calculate function and check the total reimbursed amount for Project_B
Created a measure to check the count of declined requests.
Created a slicer visual for the Project and employee
Created a bar chart for employees and reimbursement amount.
Created a pie chart for Project vs reimbursement amount
