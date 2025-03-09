# BookStoreDW-Scalable-Data-Warehouse-for-Book-Sales-
Transformed a book sales database into a data warehouse to improve data analysis, reporting efficiency, and business insights.
DB Tables description:‎

•	book: a list of all books available in the store. 

•	book_author: stores the authors for each book, which is a many-to-many ‎relationship. 

•	author: a list of all authors.‎

•	book_language: a list of possible languages of books.

•	publisher: a list of publishers for books. 

•	customer: a list of the customers of the Gravity Bookstore. 

•	customer_address: a list of addresses for customers, as a customer can have ‎more than one address, and an address has more than one customer. 

•	address: a list of addresses in the system. 

•	country: a list of countries that addresses are in.

•	cust_order: a list of orders placed by customers. 

 ![eeee](https://github.com/user-attachments/assets/38cdc433-018d-4c08-a1be-0bde160455b8)

the FactOrder table is in the center, and all the other tables (DimCustomer, ‎DimBook, DimShippingMethod, and DimDate) connect directly to it. These ‎dimension tables are flat and store all the descriptive details in one place instead of ‎being broken into smaller pieces. For example, DimBook contains everything about ‎a book, like its title, author, language, and publisher, all in one table.‎
I used a snwoflask schema because I have a bridge tables. I try to make 3 sub ‎dimension This structure makes it much faster and easier to query data since you ‎don’t need to deal with a bunch of joins. For example, if I wanted to find the total ‎sales by customer.‎
The snowflake schema also makes things easier to understand and use. Analysts or ‎anyone writing reports won’t have a hard time figuring out where the data is stored. ‎Everything is laid out clearly, with the fact table storing the numbers and the ‎dimensions holding all the details.‎

