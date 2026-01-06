# 🚀 **Todo Manager Pro** - Full Stack MERN Application

<div align="center">

![React](https://img.shields.io/badge/React-19.2-%2361DAFB?logo=react)
![Node.js](https://img.shields.io/badge/Node.js-24-%23339933?logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-7-%2347A248?logo=mongodb)
![Express](https://img.shields.io/badge/Express.js-5.2-%23000000?logo=express)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.3-%2306B6D4?logo=tailwindcss)

**A professional, production-ready Todo application with modern UI and robust backend architecture**

[Live Demo](#live-demo) • [Features](#-features) • [Tech Stack](#-tech-stack) • [Installation](#-installation) • [API Documentation](#-api-documentation)

</div>

---

## 📸 **Screenshots**

### 🎨 **Frontend - Modern UI**
| Dashboard View | Add Todo | Edit Mode |
|---------------|----------|-----------|
| <img src="https://github.com/user-attachments/assets/5eef76ae-1515-497c-a669-c10db9480c10" width="400" alt="Dashboard View"> | <img src="https://github.com/user-attachments/assets/2da3ec00-ff6c-4d68-bb69-e0640a81bb61" width="400" alt="Add Todo"> | <img src="https://github.com/user-attachments/assets/ad7fa4b9-b5a0-41bd-8928-7ee59f09dcf8" width="400" alt="Edit Mode"> |

### ⚙️ **Backend - Professional Dashboard**
| API Dashboard | Health Check |
|--------------|--------------|
| <img src="https://github.com/user-attachments/assets/3ad26b06-4c04-4b44-9ab5-cb0218da9616" width="400" alt="API Dashboard"> | <img src="https://github.com/user-attachments/assets/8a058912-4963-43e0-9c11-0055e0d4a14d" width="400" alt="Health Check"> |

---

## ✨ **Features**

### 🎯 **Frontend Features**
- ✅ **Modern UI/UX** with Tailwind CSS & glassmorphism effects
- ✅ **Real-time task management** with instant updates
- ✅ **Drag & drop task organization** (coming soon)
- ✅ **Task filtering & searching** by status/completion
- ✅ **Responsive design** for all devices (mobile, tablet, desktop)
- ✅ **Loading states & smooth animations**
- ✅ **Toast notifications** for user feedback
- ✅ **Auto-scroll to edit form** for better UX
- ✅ **Statistics dashboard** with completion rates
- ✅ **Form validation** with real-time feedback

### 🔧 **Backend Features**
- ✅ **RESTful API** with proper HTTP methods & status codes
- ✅ **MongoDB integration** with Mongoose ODM
- ✅ **Input validation & sanitization** on both client & server
- ✅ **Error handling middleware** with structured responses
- ✅ **CORS enabled** with environment-specific origins
- ✅ **Professional dashboard** with system health monitoring
- ✅ **Database connection retry logic** (auto-reconnect)
- ✅ **Multiple environment support** (dev, test, prod)
- ✅ **Graceful shutdown** handling
- ✅ **Comprehensive logging** with timestamps

### 📱 **Core Functionality**
- ✅ **Full CRUD operations** (Create, Read, Update, Delete)
- ✅ **Toggle task completion** with one-click
- ✅ **Edit tasks inline** with auto-form focus
- ✅ **Real-time statistics** (completed/pending/total tasks)
- ✅ **Task descriptions** with character limits
- ✅ **Created/Updated date tracking**
- ✅ **Confirmation dialogs** for deletions
- ✅ **Character count** for inputs

---

## 🛠️ **Tech Stack**

### **Frontend**
| Technology | Version | Purpose |
|------------|---------|---------|
| React | 19.2 | UI Library |
| Tailwind CSS | 4.1.18 | Styling Framework |
| Axios | 1.6 | HTTP Client |
| React Hot Toast | 2.4 | Notifications |
| Lucide React | 0.263 | Icons |
| Vite | 5.0 | Build Tool |

### **Backend**
| Technology | Version | Purpose |
|------------|---------|---------|
| Node.js | 24.11.1 | Runtime Environment |
| Express.js | 5.2.1 | Web Framework |
| MongoDB | 7.0.0 | NoSQL Database |
| Mongoose | 7.5 | ODM for MongoDB |
| CORS | 2.8 | Cross-Origin Resource Sharing |
| dotenv | 16.3 | Environment Variables |

---

## 🚀 **Quick Start**

### **Prerequisites**
- Node.js (v18 or higher)
- MongoDB (v7 or higher)
- npm or yarn package manager

### **Installation**

1. **Clone the repository**
```bash
git clone https://github.com/rubaiyatxeren/MERN---Todo-Manager---Full-Stack-MERN-Application.git
cd todo-manager-pro
```

2. **Backend Setup**
```bash
cd backend
npm install
# Create .env file
echo "PORT=3000" >> .env
echo "DB_URL=mongodb://localhost:27017/todo-app-db" >> .env
echo "NODE_ENV=development" >> .env
npm run dev
```

3. **Frontend Setup**
```bash
cd frontend
npm install
npm run dev
```

4. **Access the Application**
- Frontend: http://localhost:5173
- Backend API: http://localhost:3000
- API Dashboard: http://localhost:3000
- Health Check: http://localhost:3000/health

---

## 📁 **Project Structure**

### **Backend Architecture**
```
backend/
├── config/
│   └── db.js              # Database connection with retry logic
├── controllers/
│   └── todoController.js  # Business logic (optimized)
├── models/
│   └── Todo.js            # Mongoose schema with validation
├── routes/
│   └── todoRoutes.js      # API route definitions
├── middleware/
│   └── errorMiddleware.js # Global error handling
├── .env                   # Environment variables
├── package.json
└── server.js             # Express server setup
```

### **Frontend Architecture**
```
frontend/
├── src/
│   ├── components/
│   │   ├── TodoForm.jsx   # Add/edit todo form
│   │   ├── TodoItem.jsx   # Individual todo component
│   │   ├── TodoList.jsx   # Todo list container
│   │   ├── Header.jsx     # Navigation header
│   │   ├── StatsCard.jsx  # Statistics display cards
│   │   └── Footer.jsx     # Application footer
│   ├── hooks/
│   │   └── useTodos.js    # Custom hook for todo state management
│   ├── services/
│   │   └── api.js         # API service layer
│   ├── App.jsx           # Main application component
│   ├── main.jsx          # Application entry point
│   └── index.css         # Global styles & animations
├── package.json
└── tailwind.config.js    # Tailwind configuration
```

---

## 🔌 **API Documentation**

### **Base URL**
```
http://localhost:3000/api
```

### **Endpoints**

| Method | Endpoint | Description | Status Codes |
|--------|----------|-------------|--------------|
| **GET** | `/todos/all` | Get all todos | 200, 500 |
| **GET** | `/todos/:id` | Get single todo | 200, 404, 500 |
| **POST** | `/todos/create` | Create new todo | 201, 400, 500 |
| **PUT** | `/todos/update/:id` | Update todo | 200, 400, 404, 500 |
| **DELETE** | `/todos/delete/:id` | Delete todo | 200, 404, 500 |
| **PATCH** | `/todos/toggle/:id` | Toggle completion | 200, 404, 500 |
| **GET** | `/health` | System health check | 200, 503 |

### **Request/Response Examples**

**Create a Todo:**
```bash
curl -X POST http://localhost:3000/api/todos/create \
  -H "Content-Type: application/json" \
  -d '{
    "title": "Learn React Hooks",
    "description": "Master useState, useEffect, and custom hooks"
  }'
```

**Response:**
```json
{
  "success": true,
  "message": "Todo created successfully",
  "data": {
    "_id": "65a1b2c3d4e5f67890123456",
    "title": "Learn React Hooks",
    "description": "Master useState, useEffect, and custom hooks",
    "completed": false,
    "createdAt": "2024-01-15T10:30:00.000Z",
    "updatedAt": "2024-01-15T10:30:00.000Z"
  }
}
```

---

## 🎨 **UI Components**

### **TodoForm Component**
- Clean, responsive form for adding/editing todos
- Real-time character count validation
- Loading states during API calls
- Auto-focus and scroll behavior

### **TodoItem Component**
- Visual completion indicator with toggle
- Edit and delete actions with confirmation
- Created date display
- Status badge (Pending/Completed)
- Loading states for individual actions

### **StatsCard Component**
- Visual statistics display
- Color-coded status indicators
- Icon support with Lucide React
- Responsive design for all screen sizes

---

## 🔒 **Security Features**

- **Input validation** on both client and server
- **CORS configuration** with specific origins
- **Environment variables** for sensitive data
- **Error handling** without exposing stack traces
- **MongoDB injection prevention** with Mongoose
- **Request timeout** configuration
- **Connection pooling** with limits

---

## 📈 **Performance Optimizations**

### **Frontend**
- Code splitting with React.lazy()
- Optimized re-renders with proper state management
- Debounced API calls
- Minimal bundle size with tree-shaking
- Cached API responses

### **Backend**
- Database connection pooling
- Query optimization with indexes
- Response compression
- Cached responses for static endpoints
- Efficient error handling

---

## 🧪 **Testing**

```bash
# Run backend tests
cd backend
npm test

# Run frontend tests
cd frontend
npm test

# Run full test suite
npm run test:all
```

---

## 🐳 **Docker Deployment**

```dockerfile
# Backend Dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY . .
EXPOSE 3000
CMD ["node", "server.js"]
```

```bash
# Build and run with Docker Compose
docker-compose up --build
```

---

## 🌐 **Deployment**

### **Heroku Deployment**
```bash
# Backend
heroku create your-todo-backend
heroku addons:create mongolab
git push heroku main

# Frontend
npm run build
# Deploy build folder to Netlify/Vercel
```

### **Environment Variables**
```env
# Production .env
NODE_ENV=production
PORT=3000
DB_URL=mongodb+srv://username:password@cluster.mongodb.net/todo-app-prod
FRONTEND_URL=https://your-frontend-domain.com
```

---

## 🤝 **Contributing**

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### **Development Guidelines**
- Follow existing code style and patterns
- Add tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting PR

---

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 **Acknowledgments**

- [Create React App](https://create-react-app.dev/) - React bootstrapping
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [MongoDB](https://www.mongodb.com/) - NoSQL database
- [Express.js](https://expressjs.com/) - Web framework for Node.js
- [Lucide Icons](https://lucide.dev/) - Beautiful icon library
- [Vite](https://vitejs.dev/) - Next generation frontend tooling

---

## 📞 **Support**

- **Issues**: [GitHub Issues]([https://github.com/rubaiyatxeren/MERN---Todo-Manager---Full-Stack-MERN-Application/issues)
- **Email**: your-email@example.com
- **Documentation**: [API Docs](http://localhost:3000)

---

## ⭐ **Show Your Support**

If you find this project helpful, please give it a star! ⭐

[![GitHub stars](https://img.shields.io/github/stars/yourusername/todo-manager-pro?style=social)](https://github.com/yourusername/todo-manager-pro)
[![GitHub forks](https://img.shields.io/github/forks/yourusername/todo-manager-pro?style=social)](https://github.com/yourusername/todo-manager-pro/network)
[![GitHub issues](https://img.shields.io/github/issues/yourusername/todo-manager-pro)](https://github.com/yourusername/todo-manager-pro/issues)

---

<div align="center">

### **Built with ❤️ by eRubaiyat**

_"Organize your tasks, boost your productivity"_

**Happy Coding!** 🚀

</div>
