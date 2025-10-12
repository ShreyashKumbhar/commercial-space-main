# Urban Lease Platform

A modern commercial property rental platform built with Spring Boot backend and Next.js frontend.

## 📋 Table of Contents
- [Quick Start](#-quick-start)
- [Features](#-features)
- [Prerequisites](#-prerequisites)
- [Installation & Setup](#-installation--setup)
- [Running the Application](#-running-the-application)
- [Test Credentials](#-test-credentials)
- [Technical Stack](#-technical-stack)
- [Deployment](#-deployment)
- [Contributing](#-contributing)

## ⚡ Quick Start

Get the platform running in 3 simple steps:

### 1️⃣ Setup Database
```bash
# Create MySQL database
mysql -u root -p
CREATE DATABASE commercial_space;
exit;
```

### 2️⃣ Start Backend
```bash
cd backend
mvn spring-boot:run
# Backend will run on http://localhost:8080
```

### 3️⃣ Start Frontend
```bash
cd frontend
npm install
npm run dev
# Frontend will run on http://localhost:3000
```

**🎉 That's it!** Visit `http://localhost:3000` and login with test credentials below.

---

## 🚀 Features

### Authentication & User Management
- **Login/Signup**: Secure authentication with JWT tokens
- **Password Reset**: Email-based password reset functionality
- **Role-based Access**: Admin, Owner, and Customer roles
- **User Profiles**: Manage user information and preferences

### Property Management
- **Property Listing**: Add, edit, and manage commercial properties
- **Property Types**: Office, Shop, Warehouse, and Land
- **Verification System**: Admin can verify property listings
- **Search & Filter**: Advanced search by location, type, and price

### Interactive Features
- **Interactive Map**: Leaflet-based map with custom markers
- **Favorites**: Save and manage favorite properties
- **Bookings**: Request and manage property bookings
- **Inquiries**: Send inquiries to property owners
- **Reviews**: Rate and review properties with star ratings

### Modern UI/UX
- **Responsive Design**: Works on all devices
- **Modern Animations**: Smooth transitions and hover effects
- **Professional Design**: SaaS-grade interface
- **Accessibility**: WCAG AA compliant

---

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Java 17+** - [Download](https://www.oracle.com/java/technologies/downloads/)
- **Node.js 18+** - [Download](https://nodejs.org/)
- **MySQL 8.0+** - [Download](https://dev.mysql.com/downloads/)
- **Maven** - [Download](https://maven.apache.org/download.cgi)

---

## 🛠️ Installation & Setup

### Database Configuration

1. **Create Database**:
   ```sql
   CREATE DATABASE commercial_space;
   ```

2. **Update Database Credentials** (if needed):
   
   Edit `backend/src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/commercial_space
   spring.datasource.username=root
   spring.datasource.password=your_password
   ```

### Backend Setup

1. **Navigate to backend directory**:
   ```bash
   cd backend
   ```

2. **Install dependencies and run**:
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```
   
   ✅ Backend will start on `http://localhost:8080`

### Frontend Setup

1. **Navigate to frontend directory**:
   ```bash
   cd frontend
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Run development server**:
   ```bash
   npm run dev
   ```
   
   ✅ Frontend will start on `http://localhost:3000`

---

## ▶️ Running the Application

### Development Mode

**Terminal 1 - Backend:**
```bash
cd backend
mvn spring-boot:run
```

**Terminal 2 - Frontend:**
```bash
cd frontend
npm run dev
```

### Production Mode

**Backend:**
```bash
cd backend
mvn clean package
java -jar target/*.jar
```

**Frontend:**
```bash
cd frontend
npm run build
npm start
```

---

## 🧪 Test Credentials

### Admin User
- **Email**: admin@example.com
- **Password**: password123
- **Access**: Full admin dashboard, property verification

### Owner User
- **Email**: john@example.com
- **Password**: password123
- **Access**: Property management, booking requests

### Customer User
- **Email**: jane@example.com
- **Password**: password123
- **Access**: Property browsing, favorites, bookings

## 📱 Key Features

### For Customers
- Browse verified properties
- Search by location, type, and price
- Save favorite properties
- Request bookings
- Send inquiries
- Rate and review properties
- View interactive map

### For Property Owners
- List new properties
- Manage existing listings
- View booking requests
- Respond to inquiries
- Track property performance

### For Admins
- Verify property listings
- Manage all users
- Monitor platform activity
- View analytics and reports

## 🗺️ Map Features

- **Interactive Markers**: Color-coded by property type
- **Detailed Popups**: Property information with quick actions
- **Smooth Navigation**: Fly to selected properties
- **Responsive Design**: Works on mobile and desktop

## ⭐ Star Rating System

- **Interactive Stars**: Click to rate properties
- **Hover Effects**: Preview rating before clicking
- **Visual Feedback**: Clear indication of selected rating
- **Average Ratings**: Display overall property rating

## 🔧 Technical Stack

### Backend
- **Spring Boot 3.x**: Main framework
- **Spring Security**: Authentication and authorization
- **Spring Data JPA**: Database operations
- **MySQL**: Database
- **JWT**: Token-based authentication
- **JavaMailSender**: Email functionality

### Frontend
- **Next.js 14**: React framework
- **TypeScript**: Type safety
- **Tailwind CSS**: Styling
- **Framer Motion**: Animations
- **Zustand**: State management
- **React Hook Form**: Form handling
- **Leaflet**: Interactive maps

## 🚀 Deployment

### Backend Deployment
1. Build the JAR:
   ```bash
   mvn clean package
   ```
2. Run the JAR:
   ```bash
   java -jar target/*.jar
   ```

### Frontend Deployment
1. Build for production:
   ```bash
   npm run build
   ```
2. Deploy to Vercel, Netlify, or any static hosting

## 📧 Email Configuration

For password reset functionality, update the email settings in `application.properties`:
```properties
spring.mail.username=your_email@gmail.com
spring.mail.password=your_app_password
```

## 🔒 Security Features

- **JWT Authentication**: Secure token-based auth
- **Password Hashing**: BCrypt password encryption
- **Role-based Access**: Granular permissions
- **Input Validation**: Server-side validation
- **CORS Configuration**: Secure cross-origin requests

## 🎨 UI/UX Features

- **Modern Design**: Clean, professional interface
- **Responsive Layout**: Mobile-first approach
- **Smooth Animations**: Enhanced user experience
- **Accessibility**: WCAG AA compliant
- **Dark Mode Ready**: Easy theme switching

## 📊 Performance

- **Optimized Images**: WebP format support
- **Lazy Loading**: Efficient resource loading
- **Caching**: Strategic caching implementation
- **Code Splitting**: Reduced bundle sizes

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License.

---

**Happy Coding! 🚀** 