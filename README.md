---

# Experiment 5.3: E-commerce Catalog with Nested Variants (Easy Guide)

This experiment shows how to manage an e-commerce catalog with products and their variants (like color, size, stock) using a simple program. No coding knowledge is needed!

## What does it do?

- Adds sample products with different variants to the database
- Shows all products
- Filters products by category
- Shows only specific details (like color and stock) for product variants

## How to run (step by step)

1. Open your terminal
2. Type this and press Enter:
   ```bash
   node catalogDemo.js
   ```
3. You will see messages like "Inserted products", "All products", "Apparel products", and "Products with variant color and stock"

## What you will see

You will see something like:
```bash
Connected to MongoDB
Inserted products: [ ...products... ]
All products: [ ...products... ]
Apparel products: [ ...products... ]
Products with variant color and stock: [ ...projection... ]
Disconnected from MongoDB
```

## No coding needed

Just run the command above. All steps are automatic.

---


# Experiment 5.1: Product CRUD with MongoDB (Easy Guide)

This experiment shows how to manage product data using a simple program. No coding knowledge is needed!

## What does it do?

- Adds a product to the database
- Shows all products
- Updates a product
- Deletes a product

## How to run (step by step)

1. Open your terminal
2. Type this and press Enter:
   ```bash
   node crudScript.js
   ```
3. You will see messages like "Added", "Updated", and "Deleted" for products

## What you will see

You will see something like:
```bash
Connected to MongoDB
Added: { ...product info... }
All Products: [ ...list... ]
Updated: { ...product info... }
Deleted: { ...product info... }
Disconnected from MongoDB
```

---

# Experiment 5.2: Student Management System (Easy Guide)

This experiment shows how to manage student data using a simple program. You do not need to know coding to run it!

## What does it do?

- Adds 4 students to the database
- Updates 3 students
- Deletes 2 students
- Shows all results in the terminal

## How to run (step by step)

1. Open your terminal
2. Type this and press Enter:
   ```bash
   node studentCrudScript.js
   ```
3. You will see messages like "Added", "Updated", and "Deleted" for students

## What you will see

You will see something like:
```bash
Connected to MongoDB
Added: [ ...list of students... ]
All Students: [ ...list... ]
Updated: { ...student info... }
Deleted: { ...student info... }
Disconnected from MongoDB
```

## No coding needed

Just run the command above. All steps are automatic.

---

# Advanced Usage & API Endpoints

## Catalog Queries (Experiment 5.3)
- Insert products with nested variants using Mongoose
- Retrieve all products: `CatalogProduct.find()`
- Filter by category: `CatalogProduct.find({ category: 'Apparel' })`
- Project variant details: `CatalogProduct.find({}, { 'variants.color': 1, 'variants.stock': 1, name: 1 })`

For technical users, you can also use the REST API endpoints and curl commands described below for both experiments.

## Product API Endpoints (Experiment 5.1)
- `POST /products` — Add a new product
- `GET /products` — Retrieve all products
- `PUT /products/:id` — Update a product by ID
- `DELETE /products/:id` — Delete a product by ID

## Student API Endpoints (Experiment 5.2)
- `POST /students` — Add a new student
- `GET /students` — Retrieve all students
- `GET /students/:id` — Get a student by ID
- `PUT /students/:id` — Update a student by ID
- `DELETE /students/:id` — Delete a student by ID

---

## .gitignore
- Ignores `node_modules/`, `.env`, log files, and `.DS_Store`

## License
MIT
