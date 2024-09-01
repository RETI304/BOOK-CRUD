Features:
--->Create a Book: Adds a new book to the database.
--->Get Book by ID: Retrieves the details of a book by its ID.
--->Get Books with Filters**: Allows filtering of books by author, published date, and language.
--->Update a Book: Updates the details of an existing book.
--->Delete a Book: Removes a book from the databa

Requirements

---> Python 3.8+
---> Flask API
---> SQLite3

API Endpoints
1. Create a Book:
URL: /books/
Method: POST
Response: 200 OK with the created book details.

2. Get Book by ID:
URL: /books/{id}
Method: GET
Response: 200 OK with the book details, or 404 Not Found.

3.Get Books with Filters:
URL: /books/
Method: GET
Query Parameters:
author (optional)
published_date (optional)
language (optional)

4.Update a Book:
URL: /books/{id}
Method: PUT
Request Body: Same as the "Create a Book" request body.
Response: 200 OK with the updated book details, or 404 Not Found.

5.Delete a Book:
URL: /books/{id}
Method: DELETE
Response: 200 OK if the book was deleted, or 404 Not Found.

Additional Features:

Validation: Ensures fields like ISBN are unique and correctly formatted.
Error Handling: Returns appropriate HTTP status codes and error messages.
Filtering: Supports partial and case-insensitive matching for filters.
