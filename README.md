# Mercari-Price-Suggestion

Overview: 
 
Mercari is a Japanese community-powered shopping app where people can sell their stuff they don’t use but still has value. A typical listing on the website has product name, brand, category, shipping, condition, product description, and price. Sellers are allowed to choose any price for their product. This gives rise to the problem of setting the right price for a product. If the price is too high the product won’t find a buyer or if it’s too low then the seller will be getting less profit. So, if we can suggest a price for the given product listing, it helps the seller to set a better price for the product.  

 
The price of a product may depend on many factors like, brand name, demand and supply, type of product and even picture of the product. For example, electronic products of the same category and brand may have different pricing based on small changes in specifications. The task at hand is to build a machine learning model that automatically predicts the price of a product when given a product name, category, brand, shipping, product conditions, and product description.  
 
## Problem statement: 
Suggest price for a product, given name, brand name, category, shipping, item description, and condition of the product. 

## Constraints: 
● This is a kernel only challenge, hence the solution should run within 60 min and use no more than 16gb RAM. 
● Using external data is not allowed. 

## Metric: 
● The evaluation metric for this competition is Root Mean Squared Logarithmic Error. 
 
## Data:
File names: train.tsv, test.tsv The files consist of a list of product listings. These files are tab-delimited (‘\t’) 

## Columns: 
train_id or test_id - the id of the listing 

name - the title of the listing. Note that we have cleaned the data to remove text that looks like prices (e.g. $20) to avoid leakage. These removed prices are represented as [rm] 

item_condition_id - the condition of the items provided by the seller 

category_name - a category of the listing 

Brand_name - the name of the brand if available else nan 

price- the price that the item was sold for. This is the target variable that you will predict. The unit is USD. This column doesn't exist in test.tsv since that is what you will predict. 

shipping- 1 if the shipping fee is paid by seller and 0 by buyer 

item_description- the full description of the item. Note that we have cleaned the data to remove text that looks like prices (e.g. $20) to avoid leakage. These removed prices are represented as [rm] 
 
 
