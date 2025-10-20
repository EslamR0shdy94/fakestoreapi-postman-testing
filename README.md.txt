# 🧪 FakeStore API Manual Testing Project

## 📌 Description
This project focuses on **manual API testing** for [FakeStoreAPI](https://fakestoreapi.com) using **Postman**.  
It includes organized folders for testing authentication, users, products, and carts.  
Each folder contains complete CRUD (Create, Read, Update, Delete) requests with proper environment variables and test validations.

---

## 🔗 API Used
- **Base URL:** [https://fakestoreapi.com](https://fakestoreapi.com)
- **Documentation:** [https://fakestoreapi.com/docs](https://fakestoreapi.com/docs)

---

## ⚙️ Tools Used
| Tool | Purpose |
|------|----------|
| 🧰 **Postman** | For managing and executing API requests |
| ⚙️ **Environment Variables** | To store and reuse variables like `baseUrl`, `createdUserId`, `createdCartId` |
| 🧪 **Collection Runner** | To run multiple requests sequentially |
| 🧾 **Console Logs** | For debugging and tracking request info |

---

## 📂 Project Structure
FakeStoreAPI_Postman_Project/
├── Environment/
│ └── fakestore_environment.json
├── Collections/
│ └── FakeStore_API_Collection.json
├── Folders/
│ ├── Auth/
│ │ ├── Login (POST /auth/login)
│ │ └── Register (POST /users)
│ ├── Users/
│ │ ├── Get All Users (GET /users)
│ │ ├── Get Single User (GET /users/{id})
│ │ ├── Create User (POST /users)
│ │ ├── Update User (PUT /users/{id})
│ │ └── Delete User (DELETE /users/{id})
│ ├── Products/
│ │ ├── Get All Products (GET /products)
│ │ ├── Get Single Product (GET /products/{id})
│ │ ├── Add Product (POST /products)
│ │ ├── Update Product (PUT /products/{id})
│ │ └── Delete Product (DELETE /products/{id})
│ └── Carts/
│ ├── Get All Carts (GET /carts)
│ ├── Get Single Cart (GET /carts/{id})
│ ├── Create Cart (POST /carts)
│ ├── Update Cart (PUT /carts/{id})
│ └── Delete Cart (DELETE /carts/{id})
└── README.md

yaml
Copy code

---

## 🧠 Screenshots
> *(Place these screenshots inside a folder named `/screenshots`)*

### 1️⃣ Create User  
![Create User](screenshots/create_user.png)

### 2️⃣ Get All Products  
![Get Products](screenshots/get_products.png)

### 3️⃣ Create Cart  
![Create Cart](screenshots/create_cart.png)

---

## 💬 Console Logs Example
```javascript
console.log("🔹 Starting request:", pm.info.requestName);
console.log("Environment:", pm.environment.name);
console.log("Base URL:", pm.environment.get("baseUrl"));
🚀 How to Run
Open Postman

Create a new Environment named FakeStoreAPI

Add variable:
baseUrl = https://fakestoreapi.com

Import the Collection

Select the environment FakeStoreAPI

Run the whole collection via Collection Runner

Observe responses and test results

✅ Results
All endpoints were tested successfully:

Status codes validated (200, 201, 400, 404)

Request chaining with variables tested successfully

All CRUD operations completed for Users, Products, and Carts

🧑‍💻 Created by Eslam Roshdy
Manual API Testing using Postman | FakeStoreAPI