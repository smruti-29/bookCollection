Book Collection Project
Overview
The Book Collection project is a backend application built using Spring Boot, Rest API, JPA, and Hibernate. The primary purpose of this project is to allow users to manage their book collection efficiently. Users can create, update, and delete books, as well as retrieve a list of their books.

Technologies Used
Spring Boot
Rest API
JPA (Java Persistence API)
Hibernate
Features
1. Create a Book
Users can add new books to their collection by providing details such as title, author, genre, and publication year.

2. Update a Book
Users have the ability to update the information of existing books in their collection, including modifying details like title, author, genre, and publication year.

3. Delete a Book
Users can remove books from their collection, providing a streamlined way to manage their inventory.

4. List Books
Users can retrieve a list of all the books in their collection, making it easy to view and manage their reading list.

Getting Started
Clone the repository:

bash
Copy code
git clone https://github.com/smruti-29/book-collection.git
Navigate to the project directory:

bash
Copy code
cd book-collection
Build and run the application:

bash
Copy code
./mvnw spring-boot:run
The application will be accessible at http://localhost:8080.

API Endpoints
POST /api/books: Create a new book.
PUT /API/books/{id}: Update an existing book.
DELETE /api/books/{id}: Delete a book.
GET /api/books: Retrieve a list of all books.
Example Usage
Create a new book
bash
Copy code
curl -X POST -H "Content-Type: application/json" -d '{"title":"The Great Gatsby","author":"F. Scott Fitzgerald","genre":"Classic","publicationYear":1925}' http://localhost:8080/api/books
Update a book
bash
Copy code
curl -X PUT -H "Content-Type: application/json" -d '{"title":"Updated Title","author":"New Author","genre":"Fiction","publicationYear":2022}' http://localhost:8080/api/books/{id}
Delete a book
bash
Copy code
curl -X DELETE http://localhost:8080/api/books/{id}
List all books
bash
Copy code
curl http://localhost:8080/api/books
Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License.
