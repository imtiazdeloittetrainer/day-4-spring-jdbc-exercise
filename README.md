 # Spring JDBC – Exercise

## Case Study: Library Book Management System

A library wants to maintain the details of books available in the library. Develop a console-based **Library Book Management System** using **Spring JDBC**.

The application should store book details in a MySQL database and provide the following operations:

1. Add a new book.
2. Update the price of an existing book.
3. Delete a book using Book ID.
4. Display all books.
5. Search books based on category.
6. Generate a library report showing the total number of books and total available copies.

### Book Details

Each book should contain the following information:

- Book ID
- Book Name
- Author
- Category
- Price
- Available Copies

### Technical Requirements

- Configure the database connection using `DataSource`.
- Use `JdbcTemplate` for insert, update, delete, and retrieve operations.
- Use `RowMapper` to map database records to `Book` objects.
- Use `ResultSetExtractor` to generate the library report.
- Use `NamedParameterJdbcTemplate` for searching books by category.
- Take all required input dynamically from the keyboard.
- Use MySQL as the database.
- Create a `Book` class, `BookDAO` interface, and DAO implementation class.
- Do not use direct JDBC code such as `DriverManager`, `Connection`, or `PreparedStatement` in the DAO.
- Display appropriate messages after each operation.

### Sample Menu

```text
========================================
       LIBRARY BOOK MANAGEMENT
========================================

1. Add Book
2. Update Book Price
3. Delete Book
4. Display All Books
5. Search Books by Category
6. Library Book Report
7. Exit

Enter your choice:
