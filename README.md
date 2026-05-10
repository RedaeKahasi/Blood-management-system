 HEAD
# Database-Project
Blood Bank management system
# Blood Bank Management System

A comprehensive web-based blood bank management system built with Node.js, Express, React, and SQLite. This system provides role-based access control for administrators, staff, and donors to manage blood donations, requests, inventory, and appointments.

## 🚀 Features

### **For Administrators:**
- **Real-time Activity Monitoring**: Track all system activities with critical event highlighting
- **User Management**: Manage staff accounts, roles, and permissions
- **System Analytics**: View comprehensive statistics and reports
- **Blood Inventory Oversight**: Monitor blood stock levels across all blood types
- **Audit Logs**: Complete audit trail of all system activities

### **For Staff Members:**
- **Blood Request Management**: Process and fulfill blood requests
- **Inventory Management**: Add, update, and track blood inventory
- **Appointment Scheduling**: Manage donor appointments
- **Donor Management**: View and update donor information
- **Patient Records**: Manage patient information and transfusion history

### **For Donors:**
- **Personal Dashboard**: Track donation history and eligibility
- **Appointment Booking**: Schedule and manage donation appointments
- **Profile Management**: Update personal information
- **Donation History**: View complete donation records

## 🛠️ Technology Stack

### **Backend:**
- **Node.js** with Express.js
- **SQLite** database with Sequelize ORM
- **JWT Authentication** with role-based access control
- **Winston** logging system
- **Express Rate Limiting** for security

### **Frontend:**
- **React.js** with Material-UI components
- **React Router** for navigation
- **Axios** for API communication
- **Responsive Design** with Material-UI

### **Database:**
- **SQLite** for development and production
- **Sequelize** migrations for schema management
- **Comprehensive audit logging** system

## 📁 Project Structure

```
REDAE BLOOD BANK/
├── backend/                    # Backend application
│   ├── controllers/           # Route controllers
│   ├── models/               # Sequelize models
│   ├── routes/               # API routes
│   ├── services/             # Business logic services
│   ├── utils/                # Utility functions
│   ├── config/               # Database configuration
│   ├── app.js                # Express app setup
│   └── server.js             # Server entry point
├── frontend/                  # React frontend
│   ├── src/
│   │   ├── components/       # Reusable components
│   │   ├── pages/           # Page components
│   │   └── App.js           # Main app component
│   ├── public/              # Static assets
│   └── package.json
├── database/                 # Database files and schemas
├── scripts/                  # Utility scripts
├── tests/                    # Test files
├── migrations/              # Database migrations
├── logs/                    # Application logs
├── package.json             # Root package configuration
└── README.md               # This file
```

## 🚀 Quick Start

### **Prerequisites:**
- Node.js (v14 or higher)
- npm or yarn

### **Installation:**

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd "REDAE BLOOD BANK"
   ```

2. **Install backend dependencies:**
   ```bash
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd frontend
   npm install
   cd ..
   ```

4. **Set up the database:**
   ```bash
   # Run database migrations
   node scripts/run_sqlite_migration.js
   ```

5. **Create a test user (optional):**
   ```bash
   node scripts/create_test_user.js
   ```

### **Running the Application:**

1. **Start the backend server:**
   ```bash
   npm start
   ```

2. **Start the frontend (in a new terminal):**
   ```bash
   cd frontend
   npm start
   ```

3. **Access the application:**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:3001

### **Default Login Credentials:**
- **Admin**: admin@bloodbank.com / admin123
- **Staff**: staff@bloodbank.com / staff123
- **Donor**: donor@bloodbank.com / donor123

## 📊 Key Features in Detail

### **Audit Logging System**
- **Critical Activities**: Blood requests, inventory changes, role modifications
- **Normal Activities**: User logins, profile updates, routine operations
- **Real-time Monitoring**: Admin dashboard shows live activity feed
- **Comprehensive Tracking**: All user actions are logged with timestamps

### **Security Features**
- **JWT Authentication**: Secure token-based authentication
- **Role-Based Access Control**: Different permissions for admin/staff/donor
- **Rate Limiting**: Protection against brute force attacks
- **Input Validation**: Comprehensive validation on all forms

### **Blood Inventory Management**
- **Real-time Tracking**: Live inventory levels by blood type
- **Expiration Alerts**: Automatic tracking of blood expiry dates
- **Stock Alerts**: Notifications for low inventory levels
- **Usage Tracking**: Complete audit trail of blood usage

## 🔧 API Endpoints

### **Authentication:**
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `GET /api/auth/profile` - Get user profile

### **Admin Operations:**
- `GET /api/admin/dashboard` - Admin dashboard data
- `GET /api/admin/users` - User management
- `GET /api/admin/critical-activity` - Critical system activities
- `GET /api/admin/normal-activity` - Normal system activities

### **Blood Management:**
- `GET /api/blood-requests` - Blood request management
- `POST /api/blood-requests` - Create blood request
- `GET /api/inventory` - Blood inventory management
- `POST /api/donations` - Record donations

## 🧪 Testing

Run the test suite:
```bash
npm test
```

Create sample audit logs for testing:
```bash
node scripts/test_audit_logs.js
```

## 📝 Scripts

- `npm start` - Start the backend server
- `npm run dev` - Start in development mode
- `npm test` - Run test suite
- `node scripts/create_test_user.js` - Create test user
- `node scripts/test_audit_logs.js` - Create sample audit logs

## 🔒 Security

- **Password Hashing**: bcrypt with salt rounds
- **JWT Tokens**: Secure authentication tokens
- **Rate Limiting**: Protection against abuse
- **Input Sanitization**: Prevention of injection attacks
- **Role-Based Permissions**: Granular access control

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Support

For support or questions, please create an issue in the repository or contact the development team.

---

**Built with ❤️ for saving lives through efficient blood bank management**
>>>>>>> 650d10d (Initial commit)
