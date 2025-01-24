# **Library Management System API**

## **Overview**
The **Library Management System API** is a project developed in C# focusing on clean architecture, design patterns, and best practices. This API allows for the management of library resources, including books, patrons, and borrowing records.

## **Features**
- **CRUD Operations**: Manage books, patrons, and borrowing records.
- **Authentication and Authorization**: Secure API endpoints with JWT tokens.
- **Logging and Error Handling**: Comprehensive logging and graceful error handling.
- **Caching**: Improve performance with caching mechanisms.
- **Transaction Management**: Ensure data integrity with transactional operations.

## **Prerequisites**
- .NET 6.0 SDK or later
- SQL Server or any other supported database

## **Getting Started**

### **Clone the Repository**
```bash
git clone https://github.com/SOHAMD19/LibraryManagementSystemAPI.git
cd LibraryManagementSystemAPI
```

### **Configure the Database**
1. Ensure your database server is running.
2. Update the `appsettings.json` file with your database connection details:
   ```json
   "ConnectionStrings": {
       "DefaultConnection": "Server=your_server;Database=LibraryDB;User Id=your_user;Password=your_password;"
   }
   ```

### **Build and Run the Application**
1. Restore the dependencies:
   ```bash
   dotnet restore
   ```
2. Build the project:
   ```bash
   dotnet build
   ```
3. Run the application:
   ```bash
   dotnet run
   ```

### **API Endpoints**
- **Books**
  - `GET /api/books` - Retrieve all books
  - `GET /api/books/{id}` - Retrieve a book by ID
  - `POST /api/books` - Add a new book
  - `PUT /api/books/{id}` - Update a book
  - `DELETE /api/books/{id}` - Delete a book

- **Patrons**
  - `GET /api/patrons` - Retrieve all patrons
  - `GET /api/patrons/{id}` - Retrieve a patron by ID
  - `POST /api/patrons` - Add a new patron
  - `PUT /api/patrons/{id}` - Update a patron
  - `DELETE /api/patrons/{id}` - Delete a patron

- **Borrowing Records**
  - `GET /api/borrowings` - Retrieve all borrowing records
  - `GET /api/borrowings/{id}` - Retrieve a borrowing record by ID
  - `POST /api/borrowings` - Add a new borrowing record
  - `PUT /api/borrowings/{id}` - Update a borrowing record
  - `DELETE /api/borrowings/{id}` - Delete a borrowing record

## **Contributing**
Contributions are welcome! Please fork the repository and create a pull request with your changes.

## **License**
This project is licensed under the MIT License. See the LICENSE file for details.
