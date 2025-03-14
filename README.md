# MIST-4610-Project-
<img width="275" alt="image" src="https://github.com/user-attachments/assets/045ac5df-7987-4eff-baed-2e2ecbf9cf3e" />

# MIST 4610- Project 1 - Group 6
# Database Name - A.R.I.E.S BOOKSTORE
# Team Members
1. Parbatani, Sophia @sophia-parbatani
2. Wright, Ian @ianw1103
3. Pais, Ari @ari-pais
4. Harees, Reya @reyaharees
5. Nwachukwu, Esom @esom-n

# Database Description
Our Bookstore Database Management System helps to streamling bookstore operations. Management of a bookstore requires careful tracking of many different records. This includes, but is not limited to, inventory, organization, sales, and even employee information. Mantaining an efficient and easily accesible storage of this information helps the bookstore to gain important insight on the outcomes of their investments. With this database, management can keep accurate records of vital information, leading to informed decisions and more efficient operations. 
   # Data Model
This data model represents the operational structure of a bookstore, including books, inventory, sales transactions, employees, customers, genres, and publishers. At the core of the model is the Book entity, which connects to both Genre and Publisher. The Genre entity categorizes books into different types (e.g., Fiction, Non-Fiction, Mystery), while the Publisher entity stores details about the book's publishing company, such as name, contact information, and country.

The Inventory entity is directly linked to the Book entity in a one-to-one relationship, meaning that each book has only one inventory record. This ensures accurate stock tracking by monitoring quantity in stock and restock quantities.

To capture sales transactions, two interconnected tables, Sales Transactions and Book Sales Description, work together. The Sales Transactions entity records overall details of each purchase, including total price, transaction date, payment type, and the employee processing the sale. The Book Sales Description entity forms a many-to-many relationship between Sales Transactions and Books, allowing multiple books to be associated with a single sale while also enabling tracking of which books were sold in each transaction.

The Customer entity has a one-to-many relationship with Sales Transactions, meaning that a single customer can make multiple purchases over time, but each sales transaction must be linked to one specific customer. This connection is valuable for tracking customer purchasing behavior and supporting loyalty programs.

Similarly, the Employee entity has a one-to-many relationship with Sales Transactions, meaning that an employee can handle multiple sales, but each sales transaction is processed by only one employee. This relationship allows the bookstore to analyze employee performance based on sales activity. 

![image](https://github.com/user-attachments/assets/7692d766-9c74-4cba-b3d1-84dfcddb2af6)





# Data Dictionary
   
![Screenshot 2025-03-12 080618](https://github.com/user-attachments/assets/3d4f8a3b-c316-49c3-9a65-7a25529f45cf)
![Screenshot 2025-03-12 080805](https://github.com/user-attachments/assets/eb2a98ed-b842-4c16-b5a1-fd80a27e50ae)
![Screenshot 2025-03-12 080819](https://github.com/user-attachments/assets/7327a3ef-3443-4c9e-8947-a4851659958c)
![Screenshot 2025-03-12 080833](https://github.com/user-attachments/assets/02ea48b1-3bc9-450a-804f-9611f76bbfb5)

# Queries
1. Query 1 retrieves the Book title, quantity in stock, restock quantity, and total stock value (current + restock).
![image](https://github.com/user-attachments/assets/124b899f-072c-477e-a82e-1dc8513b73a9)

Functions - 
Tracks inventory to monitor stock levels,
Identifies restocking needs for low-stock books,
Optimizes supply chain by ensuring availability,
and Sorts efficiently to prioritize low-stock books,

2. Query 2 retrieves the total books sold by each publisher as well as their contact info
![image](https://github.com/user-attachments/assets/92eb1a84-76ae-4427-8a32-19a77844b1c1)

This query allows the staff to quickly identify publishers they often do business with and helps keep
Friendly contact between store and publisher may help improve/maintain business relations

3. Query 3 retrieves the total revenue generated for each book title by multiplying the quantity of books sold by the unit price using SUM.
![image](https://github.com/user-attachments/assets/5b3db0fe-8968-4cdc-bb98-48164907bbd8)

This query identifies how much revenue each book has generated based on the quantity sold, and it also identifies the books that might have the strongest sales for the book store. 

4. Query 4 retrieves the quantity in stock for each title.

![image](https://github.com/user-attachments/assets/ea76cbee-bd63-4133-877c-f8829451f394)

This query allows staff to keep track specific titles, helps maintain adequate inventory, and helps prevent loss and theft

5. Query 5 retrieves the quantity in stock for each title.

![image](https://github.com/user-attachments/assets/cbe00bd7-3a04-4d6f-a336-dc62327582f6)

6. Query 6 The query retrieves the titles and prices of books that have a price greater than 5 and were published before January 1, 2000
   
![image](https://github.com/user-attachments/assets/707d9e29-4a0c-4cde-8d61-bfe5dfe31351)

This query helps bookstores and libraries determine which older books are still valuable, in demand, and worth restocking. It can also be useful for pricing decisions, such as determining if older books should be discounted or promoted.

7. Query 7 This Query retrieves the title name and corresponding author of a book in alphabetical order 

![image](https://github.com/user-attachments/assets/5782525c-b5e1-479e-b076-c748cb2f7aea)

This query helps employees/customers efficiently locate books and aids management of inventory and representation of each author.

8. Query 8 retrieves a list of publishers along with their contact emails and the total number of books they have sold, ranked in descending order of sales.
<img width="369" alt="image" src="https://github.com/user-attachments/assets/d77e2398-1d93-4424-acf4-7442c52a4005" />

This query allows bookstore staff to identify top-selling publishers, helping with inventory decisions, supplier negotiations, and restocking popular books.

9. Query 9 retrieves all books that belong to a specific genre, helping bookstore managers see the available titles.
<img width="323" alt="image" src="https://github.com/user-attachments/assets/2bd32241-7091-483a-b59c-690c43882f6f" />

This query helps managers check inventory for a particular genre. It's also useful for recommending books to customers, and ensures all books under the selected genre are displayed.

10. Query 10 retrieves the contact information to all employees as well as employee id.
<img width="237" alt="image" src="https://github.com/user-attachments/assets/d7d0a532-a168-405b-ac5b-19a5d3483f8a" />

This query help bookstore staff be able to quickly identify employee contact info, and allows management to distribute information through mass emails or personal messages with efficiency. 

# Database information:

![image](https://github.com/user-attachments/assets/6082d593-e421-4da2-9d46-84516670d67c)

Name of the database is ha_group6





