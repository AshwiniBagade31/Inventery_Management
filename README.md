
# Product CRUD Application

## Description
This is a Product CRUD (Create, Read, Update, Delete) application built using Node.js and Express. It allows users to manage products with basic features like registration, login, and product management.

## Features
- User registration and authentication.
- Product management (add, update, delete).
- Session management using `express-session`.
- Uploading product images with `multer`.
- EJS templating for rendering views.

## Installation
1. Clone the repository to your local machine.
2. Install the required dependencies using the following command:npm install
  
The application will run on port 3000 by default.

## Usage
1. Visit `http://localhost:3000/register` to create a new user account.
2. Log in using your credentials at `http://localhost:3000/login`.
3. Once logged in, you can:
- View the list of products at `http://localhost:3000/`.
- Add a new product at `http://localhost:3000/add-product`.
- Update a product at `http://localhost:3000/update-product/:id` (replace `:id` with the product's ID).
- Delete a product by submitting a POST request to `/delete-product/:id`.

## Controllers
The application is structured with the following controllers:

### `ProductsController`
- `getProducts(req, res, next)`: Retrieves and renders a list of products.
- `getAddProduct(req, res, next)`: Renders the view for adding a new product.
- `postAddProduct(req, res, next)`: Handles the addition of a new product.
- `getUpdateProductView(req, res, next)`: Renders the view for updating a product.
- `postUpdateProduct(req, res)`: Handles the update of a product.
- `deleteProduct(req, res)`: Handles the deletion of a product.

### `UserController`
- `getRegister(req, res)`: Renders the registration view.
- `getLogin(req, res)`: Renders the login view.
- `postRegister(req, res)`: Handles user registration.
- `postLogin(req, res)`: Handles user login and session management.
- `logout(req, res)`: Logs out the user and destroys the session.

## Configuration
You can configure the application by modifying settings in the `index.js` file. Make sure to set up a proper database connection and session management based on your requirements.

## Dependencies
- [Express](https://www.npmjs.com/package/express)
- [Express Session](https://www.npmjs.com/package/express-session)
- [Multer](https://www.npmjs.com/package/multer)
- [EJS](https://www.npmjs.com/package/ejs)
- [Express EJS Layouts](https://www.npmjs.com/package/express-ejs-layouts)
- [Cookie Parser](https://www.npmjs.com/package/cookie-parser)

## License
This project is licensed under the ISC License. 



