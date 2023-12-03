# 1. Project Motivation

The main objective of this project is to examplify basic steps that could be taken by any novice Data Scientist to address select business questions.
Here, an imaginary scenario is conjured whereupon some entrepreneur wishes to open a simple goods shop in Istanbul and part of their research, emply 
a Data Scientist to help answer the following questions:
1.1 What might be the best location to setup a new shop?
1.2 What goods might be worthwhile selling?
1.3 Would the selected goods appeal more to males or females, or both equally?
These questions form the basis of *Business Understanding*

# 2. How to Prepare a Responce

To answer these questions, the scientist seeks the appropriate data either by collecting it first-hand or obtained from existing sources.
For this project, the data already exists and is sourced from Istanbul's Customer Shopping Data sourced from 
https://www.kaggle.com/datasets/mehmettahiraslan/customer-shopping-dataset, (Aslan, 2023).

# 3. Data Wrangling and Cleaning

3.1 To determine the best mall for the entrepreneur, consider analyzing the 3 columns including the shopping_mall, price and quantity.
	If the mall name is missing or price or quantity <= 0, drop the row as it does not help answer the question.
3.2 Here, the columns of interest would be category and quantity. So if category is missing or quantity <= 0, remove row from analysis.
3.3 This question demands investigating gender and quantity of products purchaed. As such, rows of missing gender or quantity <= 0 are ignored.

# 4. Data Analysis

For all analyses, the following Python libraries were used:numpy, pandas, matplotlib.pyplot and seaborn

# 5. Results, Interpretation and Conclusion

Though much of the analysis carried out is descriptive, the results are nevertheless sufficient to address the questions asked. 
5.1 For the first question, the weighted average item cost price per mall was found to be roughly the same 
	 across malls at around 842. So, based on the quantity of goods sold, the Mall of Istanbul would be found to be the best location 
	 with most sold units making up about 20.1% of all units, with Kanyon close behind at 19.9%. 
  
	 ![Proportion_of_Units_Sold_per_Mall](https://github.com/BrianMekiSCA/BrianMekiSCA.github.io/assets/53751214/519f6c74-a686-4e60-b94f-23450dbe7931)
	 
5.2 The product categories to invest in once the shop is located in the Mall of Istanbul include Clothing, Cosmetics and Food&Beverage. This is because these three categories 
result in approximately 65% of all products sold with each claiming 35%, 15% and 15% respectively. 
	
5.3 On average, both males and females are found to consume roughly the same quantity of products at 3 units with females showing slighly more variability with a standard deviation
of about 1.41 vs. 1.40 for males.  

# 6. Conclusion
   
Based on the Customer Shopping Data (Aslan, 2023), the entrepreneur will do well to locate their shop in the Mall of Istanbul where they can should prioritize selling 
Clothing, Cosmetics and Food & Beverage to maximize profitability. Sustainability should be easier to achieve as long as they cater equally to both males and females.

# 7. Supporting Material

A collection of files is accompanies this project. These include:
* a copy of the Customer Shopping Data (Aslan, 2023) in CSV format,
* plot outputs showing proportion of units sold per mall and per product category respectively,
