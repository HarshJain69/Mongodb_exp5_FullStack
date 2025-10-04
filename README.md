# MongoDB Product CRUD Example

This Node.js application demonstrates CRUD operations for a Product database using Express and Mongoose, with MongoDB as the backend.

## Features
- Product model: `name`, `price`, `category`
- REST API for Create, Read, Update, Delete
- CLI script for automated CRUD operations
- Uses environment variables for configuration

## Setup
1. **Clone the repository**
2. **Install dependencies**
   ```sh
   npm install
   ```
3. **Configure MongoDB**
   - Set your MongoDB URI in `.env`:
     ```
     MONGO_URI=your_mongodb_uri
     PORT=3000
     ```

## Usage
### Start the server
```sh
npm start
```

### Run CRUD script
```sh
node crudScript.js
```

### API Endpoints
- `POST /products` — Add a new product
- `GET /products` — Retrieve all products
- `PUT /products/:id` — Update a product by ID
- `DELETE /products/:id` — Delete a product by ID

#### Example curl commands
```sh
# Add a product
curl -X POST http://localhost:3000/products -H "Content-Type: application/json" -d '{"name":"Sample Product","price":99.99,"category":"Electronics"}'

# Get all products
curl http://localhost:3000/products

# Update a product
curl -X PUT http://localhost:3000/products/<PRODUCT_ID> -H "Content-Type: application/json" -d '{"name":"Updated Name","price":79.99,"category":"Gadgets"}'

# Delete a product
curl -X DELETE http://localhost:3000/products/<PRODUCT_ID>
```

## Scripts
- `crudScript.js`: Runs all CRUD operations in sequence using Node.js

## .gitignore
- Ignores `node_modules/`, `.env`, log files, and `.DS_Store`

## License
MIT
