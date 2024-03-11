# DB-Assignment
# 1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram?
Both the "Product" and "Product_Category" entities have a one-to-many relation. This means that a single product can belong to one category, but a category can include several items. 
Detail Explanation.
1. In the 'Product_Category' database, there is a primary key named 'id' and a foreign key known as 'category_id' for each product.
2.The "category_id" contains the name and information description.

# 2.  How could you ensure that each product in the "Product" table has a valid category assigned to it?
There are several ways to do this. One of the ways follows.
Foreign Key Constraint: To achieve the most reliable and common approach, it's best to define a FOREIGN KEY constraint on the 'category_id' column of the 'Product' table. This constraint would reference the primary key ("id") of the "Product_Category" table. This enforces data integrity at the database level, preventing products from being inserted with invalid category IDs.
