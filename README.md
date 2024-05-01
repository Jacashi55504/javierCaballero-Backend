# VoidVials Backend
This project serves as the backend for the VoidVials platform, a visionary enterprise that provides rare and high-quality substances for a diverse clientele. Developed using Node.js with Express and MongoDB, this backend supports a full range of CRUD operations for product management. 

## Features
- **Product Management**: Allows the addition, deletion, update, and retrieval of product details.
- **Data Integrity**: Ensures that all product entries are unique and meet predefined criteria.
- **Search Functionality**: Offers the ability to search for products based on various attributes.

## Architecture
The project is structured as follows:
- `controllers`: Functions that directly interact with the database.
- `models`: Defines the data schema for products.
- `routes`: Manages the API endpoints.
- `config`: Contains database configuration and connection setup.
- `middleware`: Includes error handling and other middleware functions.
- Root file: `server.js`

## Prerequisites
Before running this project locally, ensure you have:
- Node.js installed.
- MongoDB account set up in MongoDB Atlas.
- Postman for testing API endpoints.

### Environment Setup
Create a `.env` file in the root directory of the project. It should contain the following:
```properties
NODE_ENV=development
PORT=8000 
MONGO_URI=your_mongodb_connection_string_here
```

Replace `your_mongodb_connection_string_here` with your actual MongoDB Atlas connection string. This connection string is crucial for enabling the backend to connect to your MongoDB database.

## Running the Application
To run the application locally, follow these steps:
1. Clone the repository to your machine.
2. Navigate to the project directory in the terminal.
3. Install the required Node.js packages:
```bash
npm install
```
4. Start the server:
```bash
npm start
```
5. The server will run on http://localhost:8000. Use Postman to test the API endpoints.

## API Endpoints
The application supports the following endpoints:
- **GET `/api/products`**: Retrieve all products.
- **POST `/api/products`**: Add a new product.
- **PUT `/api/products/:id`**: Update an existing product.
- **DELETE `/api/products/:id`**: Remove a product.

Each endpoint allows you to manage the product inventory effectively, from creating new entries to updating and deleting existing ones.

Javier CS






