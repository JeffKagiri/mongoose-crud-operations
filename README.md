# Mongoose CRUD Operations

This project demonstrates **basic CRUD operations** (Create, Read, Update, Delete) using **Node.js**, **Express**, and **Mongoose** connected to a **MongoDB Atlas** database.

## Features

* Connects to MongoDB Atlas using Mongoose
* Defines a `Person` model with `name`, `age`, and `favoriteFoods` fields
* Performs the following operations:

  * Create and save a single document
  * Create multiple documents at once
  * Find documents by name
  * Find one document by a favorite food
  * Find documents by ID
  * Update documents (classic find-edit-save and `findOneAndUpdate`)
  * Delete one document by ID
  * Delete many documents by name
  * Complex query: filter by favorite food, sort, limit, and select specific fields

## Project Structure

```
mongoose-crud-operations/
├─ server.js           # Main server and CRUD operations
├─ package.json        # Project dependencies
├─ .env                # Environment variables (MongoDB URI)
├─ .gitignore          # Ignored files and folders
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/JeffKagiri/mongoose-crud-operations.git
   ```

2. Navigate to the project folder:

   ```bash
   cd mongoose-crud-operations
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the root folder with your MongoDB Atlas URI:

   ```
   MONGO_URI='your_mongodb_atlas_connection_string'
   ```

## Usage

Run the server:

```bash
node server.js
```

* Uncomment the function calls at the bottom of `server.js` to run specific CRUD operations.
* Check the console for output of each operation.

## Notes

* Do not commit your `.env` file or `node_modules` to GitHub.
* The project demonstrates **asynchronous operations** with Mongoose using `async/await`.

## License

This project is open-source and free to use.
