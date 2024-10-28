# E-commerce RESTful API

This is an E-commerce RESTful API built using Node.js, Express, and MongoDB. This API provides endpoints for handling categories, brands, products, users, and other core features of an e-commerce platform.

## Features

- **User Authentication**: Secure signup and login, password reset, and email verification.
- **Product Management**: Create, update, delete, and view products with support for filtering and sorting.
- **Category & Brand Management**: Add, edit, and delete categories and brands.
- **Cart and Orders**: Manage user carts and place orders.
- **Wishlist**: Allow users to add and remove products from their wishlist.
- **Reviews**: Users can add reviews for products.
- **Coupons**: Apply discounts via coupons.
- **Address Book**: Store user addresses for faster checkouts.

## API Documentation

Each endpoint requires a unique URL structure and may require authorization tokens, particularly for actions like creating, updating, and deleting resources. The following is an overview of the key endpoints.

### Categories

- **Get Categories**: `GET /api/v1/categories`
- **Get Category by ID**: `GET /api/v1/categories/:id`
- **Create Category** (Admin only): `POST /api/v1/categories`
- **Update Category** (Admin only): `PUT /api/v1/categories/:id`
- **Delete Category** (Admin only): `DELETE /api/v1/categories/:id`

### Brands

- **Get Brands**: `GET /api/v1/brands`
- **Get Brand by ID**: `GET /api/v1/brands/:id`
- **Create Brand** (Admin only): `POST /api/v1/brands`
- **Update Brand** (Admin only): `PUT /api/v1/brands/:id`
- **Delete Brand** (Admin only): `DELETE /api/v1/brands/:id`

### Products

- **Get Products**: `GET /api/v1/products`
- **Get Product by ID**: `GET /api/v1/products/:id`
- **Create Product** (Admin only): `POST /api/v1/products`
- **Update Product** (Admin only): `PUT /api/v1/products/:id`
- **Delete Product** (Admin only): `DELETE /api/v1/products/:id`

### Users (Admin)

- **Get Users**: `GET /api/v1/users`
- **Get User by ID**: `GET /api/v1/users/:id`
- **Create User**: `POST /api/v1/users`
- **Update User**: `PUT /api/v1/users/:id`
- **Delete User**: `DELETE /api/v1/users/:id`

### Authentication

- **Sign Up**: `POST /api/v1/auth/signup`
- **Login**: `POST /api/v1/auth/login`
- **Forgot Password**: `POST /api/v1/auth/forgotpassword`
- **Reset Password**: `PUT /api/v1/auth/resetpassword`

### Cart

- **Add Product to Cart**: `POST /api/v1/cart`
- **Get User's Cart**: `GET /api/v1/cart`
- **Update Cart Item Quantity**: `PUT /api/v1/cart/:itemId`
- **Remove Cart Item**: `DELETE /api/v1/cart/:itemId`
- **Clear Cart**: `DELETE /api/v1/cart/clear`

### Orders

- **Place Order**: `POST /api/v1/orders`
- **Get User Orders**: `GET /api/v1/orders/user`

### Coupons

- **Get Coupons**: `GET /api/v1/coupons`
- **Create Coupon** (Admin only): `POST /api/v1/coupons`
- **Update Coupon** (Admin only): `PUT /api/v1/coupons/:id`
- **Delete Coupon** (Admin only): `DELETE /api/v1/coupons/:id`

## Authentication

Authentication is managed using JWT tokens. Include the JWT token in the `Authorization` header as `Bearer <token>` for endpoints requiring authentication.

## Error Handling

API responses include error messages for invalid requests, unauthorized actions, and missing resources. Ensure to handle errors as they arise when interacting with this API.

---

This README provides an overview based on your API’s Postman collection. If you need further customization or details, please let me know!
