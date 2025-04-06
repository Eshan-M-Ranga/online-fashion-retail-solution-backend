
# 🛒 Fashion Retail with Customer-Focused Product Suggestions-Backend

This is the backend service for the Fashion Retail application, developed using Node.js and Express.js. It serves as the RESTful API handling all client requests, managing operations related to user, employee, and inventory management. Data is stored in MongoDB Atlas, and the backend also facilitates image uploads to Cloudinary cloud storage.

---

## 🚀 Features

- **User Management**: Handles user authentication and authorization with role-based access control using JWT.
- **Employee Management**: Manages employee records and their respective roles within the system.
- **Inventory Management**: Oversees product listings, stock levels, and supplier information.
- **Image Uploads**: Processes and uploads images to Cloudinary for efficient storage and retrieval.
- **CORS Support**: Implements Cross-Origin Resource Sharing to allow secure interactions with the frontend application.

---

## 🛠️ Tech Stack

- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB Atlas
- **Authentication**: JSON Web Tokens (JWT)
- **ORM**: Mongoose
- **Environment Variables**: dotenv
- **File Uploads**: multer, busboy
- **Cloud Storage**: Cloudinary

---

## 📂 Folder Structure

```
online-fashion-retail-solution-backend/ 
├── EmployeeManagement/ 
├── UserManagement/ 
├── inquiryManagement/ 
├── inventoryStockSupplierManagement/ 
├── middleware/ 
├── models/ 
├── .gitignore 
├── README.md 
├── authController.js 
├── authRoute.js 
├── cartRouter.js 
├── commentRouter.js 
├── controller.js 
├── orderRouter.js 
├── package-lock.json 
├── package.json 
├── router.js 
└── server.js
```
---

## 🔑 Environment Variables

Create a `.env` file in the root directory and include the following variables with your own credentials:

```env
MONGO_URI=your_mongodb_atlas_connection_string
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
JWT_SECRET=your_jwt_secret_key
```

---

## ⚙️ Getting Started

### Prerequisites

- Node.js installed on your machine
- npm (Node Package Manager)
- MongoDB Atlas account with a configured database
- Cloudinary account for image storage

---

## 🧩 Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Eshan-M-Ranga/online-fashion-retail-solution-backend.git
   cd online-fashion-retail-solution-backend
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Set up environment variables:**

   Create a .env file in the root directory and add your MongoDB Atlas and Cloudinary credentials as specified above.

4. **Start the server:**

   ```bash
   npm start
   ```
   
   The server will run on http://localhost:3000 by default.

---

## 🔗 API Endpoints

The backend exposes the following main API endpoints:

- User Management:

  - `POST /api/users/register`: Register a new user

  - `POST /api/users/login`: Authenticate a user and return a JWT

  - `GET /api/users/profile`: Retrieve user profile information

- Employee Management:

  - `POST /api/employees/`: Add a new employee

  - `GET /api/employees/`: Retrieve all employees

  - `PUT /api/employees/:id`: Update employee details

  - `DELETE /api/employees/:id`: Remove an employee

- Inventory Management:

  - `POST /api/products/`: Add a new product

  - `GET /api/products/`: Retrieve all products

  - `PUT /api/products/:id`: Update product information

  - `DELETE /api/products/:id`: Delete a product

- Image Uploads:

  - `POST /api/upload/`: Upload an image to Cloudinary

  Note: Detailed API documentation and additional endpoints can be found by inspecting the route files.

---

## 🛡️ Authentication & Authorization
  - JWT Authentication: Secure endpoints using JSON Web Tokens. Ensure that the Authorization header contains a valid token.

  - Role-Based Access Control: Differentiate access permissions based on user roles.


---

## ⚠️ Special Notes
 - CORS Configuration: The server is configured to handle Cross-Origin Resource Sharing.

 - Cloudinary Integration: Set up .env with valid Cloudinary credentials.

 - Environment Setup: Restart the server after making changes to environment variables.


---

## 🧑‍💻 Author
**Eshan M Ranga**

- GitHub: [@Eshan-M-Ranga](https://github.com/Eshan-M-Ranga)
- LinkedIn: [Eshan M Ranga](https://www.linkedin.com/in/eshan-m-ranga/)


---

## 🙌 Contributing
 - Fork the repository.

 - Create a new branch (git checkout -b feature/YourFeature).

 - Commit your changes (git commit -m 'Add some feature').

 - Push to the branch (git push origin feature/YourFeature).

 - Open a Pull Request.


---

## 💬 Feedback
For suggestions or issues, please open an issue in the repository or contact me directly via GitHub.



