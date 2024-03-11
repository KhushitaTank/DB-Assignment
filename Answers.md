# DB-Assignment
# 1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram?
Both the "Product" and "Product_Category" entities have a one-to-many connection. This means that a single product can be assigned to one category, but a category can include several items. 
Detail Explanation
A product contains a foreign key "category_id" that refers to the primary key "id" in the "Product_Category" database.
The "category_id" field identifies which category a certain product belongs to.

# 2.  How could you ensure that each product in the "Product" table has a valid category assigned to it?
