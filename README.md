
# **Express MongoDB CRUD API**

## **Overview**

This project is a basic CRUD (Create, Read, Update, Delete) API built using **Express.js** and **MongoDB**. It allows users to interact with a MongoDB database by performing operations like adding new records, retrieving all records, fetching a specific record by ID, updating records, and deleting records. The API is built with simplicity and ease of understanding in mind, making it a great starting point for learning backend development with Node.js and MongoDB.

## **Technologies Used**

- **Node.js**: JavaScript runtime environment used for server-side scripting.
- **Express.js**: Minimalist web framework for Node.js, used to build the API.
- **MongoDB**: NoSQL database used to store and manage data.
- **Mongoose**: ODM (Object Data Modeling) library for MongoDB and Node.js, used to interact with the MongoDB database.
- **body-parser**: Middleware to parse incoming request bodies in a middleware before your handlers.

## **Setup and Installation**

### **Prerequisites**

- **Node.js** and **npm** installed on your machine.
- **MongoDB** installed or access to a MongoDB Atlas cluster.
- Create a `.env` file at the root of your project and add the following line:

  ```plaintext
  DATABASE_URL=<Your MongoDB connection string>
  ```

### **Installation Steps**

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/express-mongodb-crud-api.git
   cd express-mongodb-crud-api
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Start the Server**

   ```bash
   npm start
   ```

   The server will start running on `http://localhost:3000`.

## **Project Structure**

- `index.js`: The main entry point of the application. It sets up the Express server, connects to MongoDB, and defines the middleware and routes.
- `routes/routes.js`: Defines the API endpoints and handles HTTP requests for creating, reading, updating, and deleting data.
- `models/model.js`: Defines the MongoDB schema and model used to interact with the MongoDB database.

## **API Endpoints**

### **POST /api/post**

- **Description**: Adds a new document to the MongoDB collection.
- **Request Body**:
  ```json
  {
    "name": "John Doe",
    "age": 30
  }
  ```
- **Response**: Returns the created document.

### **GET /api/getAll**

- **Description**: Retrieves all documents from the MongoDB collection.
- **Response**: Returns an array of all documents.

### **GET /api/getOne/:id**

- **Description**: Retrieves a single document by its ID.
- **Params**:
  - `id` (String): The ID of the document to retrieve.
- **Response**: Returns the document with the specified ID.

### **PATCH /api/update/:id**

- **Description**: Updates a document by its ID.
- **Params**:
  - `id` (String): The ID of the document to update.
- **Request Body**: JSON object containing the fields to update.
- **Response**: Returns the updated document.

### **DELETE /api/delete/:id**

- **Description**: Deletes a document by its ID.
- **Params**:
  - `id` (String): The ID of the document to delete.
- **Response**: Confirmation message with the name of the deleted document.

## **Running the Project**

1. **Start the Server**

   ```bash
   npm start
   ```

   This will run the server on `http://localhost:3000`.

2. **Using the API**
   You can use tools like **Postman** or **cURL** to interact with the API endpoints listed above.

## **Error Handling**

The API includes basic error handling to ensure that meaningful error messages are returned when something goes wrong, such as when a resource is not found or a request is malformed.

## **Contributing**

If you'd like to contribute to this project, feel free to fork the repository, create a new branch, and submit a pull request. Contributions, improvements, and bug fixes are always welcome!


## **Contact**

For any questions or feedback, feel free to reach out via jadwaniprem12@gmail.com.


