LibraryManagementSystemAPI
Welcome to the Library Management System API! This project aims to facilitate the seamless management of library resources. With this API, you can efficiently manage books, users, and library operations.

Features:
Book Management: Easily add, update, remove, and search books.
User Management: Manage user registrations, updates, and removals.
Borrow/Return Management: Track borrowing and returning of books.
Authentication: Secure login and user authentication.
Admin Dashboard: A robust dashboard for librarian/admin use
Running the API
Once the server is running, you can access the API at http://127.0.0.1:8000/.

Sample Requests
Authentication
Register a new user
sh
POST /api/register/
{
  "username": "testuser",
  "password": "testpass123"
}
Login a user
sh
POST /api/login/
{
  "username": "testuser",
  "password": "testpass123"
}
Book Management
Add a new book
sh
POST /api/books/
{
  "title": "1984",
  "author": "George Orwell",
  "isbn": "9780451524935",
  "copies": 5
}
Get details of all books
sh
GET /api/books/
Get details of a specific book
sh
GET /api/books/{id}/
Update details of a book
sh
PUT /api/books/{id}/
{
  "title": "1984",
  "author": "George Orwell",
  "isbn": "9780451524935",
  "copies": 7
}
Delete a book
sh
DELETE /api/books/{id}/
User Management
View all users
sh
GET /api/users/
Get details of a specific user
sh
GET /api/users/{id}/
Borrow/Return Management
Borrow a book
sh
POST /api/borrow/
{
  "user_id": 1,
  "book_id": 101
}
Return a book
sh
POST /api/return/
{
  "user_id": 1,
  "book_id": 101
}    
