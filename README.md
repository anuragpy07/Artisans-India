# 🎨 Artisan India - E-Commerce Marketplace

<div align="center">
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
</div>

<div align="center">
  <h3>🚀 Connecting Local Artisans with Global Customers</h3>
  <p>A modern, full-stack marketplace platform showcasing India's rich heritage of handmade crafts and artisan products</p>
</div>

---

## 🌟 Features

### 👥 **User Experience**
- 🛍️ **Browse & Shop** - Discover unique handmade products from local artisans
- 🛒 **Smart Cart** - Add/remove items with real-time updates
- 🔐 **Secure Authentication** - JWT-based sign up and login system
- 📊 **Personal Dashboard** - Track orders, manage profile, and view purchase history
- 🎯 **Product Filtering** - Find exactly what you're looking for

### 🏪 **Seller Portal**
- 📝 **Multi-Step Registration** - Streamlined seller onboarding process
- ✅ **Live Validation** - Real-time form validation with progress tracking
- ⏳ **Admin Approval System** - Quality control through admin verification
- 📈 **Seller Dashboard** - Manage products and track sales

### ⚙️ **Admin Panel**
- 👨‍💼 **Seller Management** - Approve or reject seller applications
- 📋 **Clean Interface** - Intuitive admin dashboard for easy management
- 🔍 **Application Review** - Detailed seller application screening

## 🗺️ Page Structure

| Route | Description | Access Level |
|-------|-------------|--------------|
| `/` | 🏠 Landing page with welcome banner | Public |
| `/signin` | 🔑 User login form | Public |
| `/signup` | ✍️ New user registration | Public |
| `/shop` | 🛍️ Product catalog from artisans | Public |
| `/artisans` | 👥 Artisan directory with filters | Public |
| `/cart` | 🛒 Shopping cart management | User |
| `/dashboard` | 📊 User profile & order history | User |
| `/register-as-seller` | 📝 Seller application form | User |
| `/admin` | ⚙️ Admin panel for approvals | Admin |

## 🛠️ Tech Stack

### **Frontend**
- ⚛️ **React.js** - Modern UI library
- 🌐 **React Router** - Client-side routing
- 🔄 **Context API** - State management
- 📡 **Axios** - HTTP client
- 🎨 **Tailwind CSS** - Utility-first styling
- 🎯 **React Icons** - Beautiful icon library

### **Backend**
- 🟢 **Node.js** - Server runtime
- ⚡ **Express.js** - Web framework
- 🍃 **MongoDB** - NoSQL database
- 🔐 **JWT** - Authentication tokens
- 🔒 **bcrypt** - Password hashing

## 📡 API Endpoints

### **Authentication**
```
POST /api/signup     - Register new user
POST /api/signin     - User login
```

### **Seller Management**
```
POST /api/sellers           - Submit seller application
GET /api/sellers/pending    - Fetch pending applications
PATCH /api/sellers/:id/approve - Approve/reject seller
```

### **Products & Cart**
```
GET /api/products    - Fetch all products
POST /api/cart       - Add item to cart
GET /api/cart        - Retrieve user cart
```

## 📁 Project Structure

```
artisan-india/
├── 📁 frontend/
│   ├── 📁 src/
│   │   ├── 📁 components/
│   │   │   ├── Home.jsx
│   │   │   ├── SignIn.jsx
│   │   │   ├── SignUp.jsx
│   │   │   ├── Shop.jsx
│   │   │   ├── Artisans.jsx
│   │   │   ├── Cart.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   ├── RegisterAsSeller.jsx
│   │   │   └── AdminDashboard.jsx
│   │   ├── 📁 context/
│   │   │   └── AuthContext.js
│   │   ├── 📁 styles/
│   │   └── App.js
├── 📁 backend/
│   ├── 📁 models/
│   ├── 📁 routes/
│   ├── 📁 middleware/
│   └── server.js
└── README.md
```

## 🚀 Quick Start

### **Prerequisites**
- Node.js (v14 or higher)
- MongoDB (local or cloud)
- Git

### **Installation**

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/artisan-india.git
   cd artisan-india
   ```

2. **Setup Frontend**
   ```bash
   cd frontend
   npm install
   npm start
   ```
   Frontend runs on `http://localhost:3000`

3. **Setup Backend**
   ```bash
   cd backend
   npm install
   ```

4. **Environment Configuration**
   Create `.env` file in backend directory:
   ```env
   MONGO_URI=your-mongodb-connection-string
   JWT_SECRET=your-super-secret-key
   PORT=5000
   ```

5. **Start Backend Server**
   ```bash
   npm run dev
   ```
   Backend runs on `http://localhost:5000`

## 🔐 Authentication Flow

- **JWT-based** secure authentication
- **AuthContext** manages user sessions across components
- **Protected routes** for dashboard and admin access
- **Role-based** access control (User/Seller/Admin)

## 🎨 Design Philosophy

- **Mobile-first** responsive design
- **Figma-inspired** UI components
- **Clean & intuitive** user experience
- **Accessibility** focused development
- **Performance** optimized React components

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- **Icons**: FontAwesome & React Icons
- **UI/UX**: Figma design system
- **Community**: React and Node.js communities
- **Inspiration**: Supporting local artisans and traditional crafts

---

<div align="center">
  <p>Made with ❤️ for Indian Artisans</p>
  <p><strong>Artisans India</strong> - Preserving Heritage, Embracing Technology</p>
</div>

## 📊 Project Status

- [x] Frontend setup with React
- [x] Backend API with Express & MongoDB
- [x] User authentication system
- [x] Seller registration workflow
- [x] Admin approval system
- [ ] Payment integration
- [ ] Order management
- [ ] Email notifications
- [ ] Advanced search & filters

## 🔗 Links

- **Live Demo**: [Coming Soon]
- **API Documentation**: [Coming Soon]
- **Design System**: [Figma Link]

---

*⭐ If you found this project helpful, please give it a star! It helps others discover the project.*
