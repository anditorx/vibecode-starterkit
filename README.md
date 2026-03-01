# VibeCoding Starter Kit - @anditorx GoClean Web App

## 🚀 Overview

VibeCoding Starter Kit is a comprehensive full-stack web application template designed for building modern GoClean management systems. This project provides a complete foundation with a Go Fiber backend and React TypeScript frontend, following industry best practices and clean architecture principles.

## 🎯 Project Purpose

This starter kit is specifically designed for:

- **GoClean Business Management**: Complete CRM for GoClean service providers
- **Admin Dashboard**: Comprehensive management interface for business operations
- **Customer Portal**: Modern landing page and service catalog for customers
- **Learning Platform**: Educational template for full-stack development best practices

## 🏗️ Architecture Overview

### Backend (Go Fiber + GORM)

- **Framework**: Go Fiber v2 - High performance web framework
- **ORM**: GORM with PostgreSQL support
- **Authentication**: JWT with bcrypt password hashing
- **Database**: PostgreSQL with soft delete support
- **API Structure**: RESTful API with consistent response format

### Frontend (React + TypeScript + Vite)

- **Framework**: React 18+ with TypeScript
- **Build Tool**: Vite 6+ for fast development
- **Styling**: Tailwind CSS v3 with custom design system
- **UI Components**: Shadcn UI for consistent component library
- **State Management**: Zustand for global state
- **API Client**: Axios with interceptors
- **PWA Ready**: Progressive Web App capabilities

## 📁 Project Structure

```
vibecoding-starterkit/
├── backend/                 # Go Fiber Backend
│   ├── cmd/                # Application entry points
│   ├── config/             # Configuration loading
│   ├── database/           # Database connection & migrations
│   ├── handlers/           # HTTP handlers (controllers)
│   ├── middleware/         # Fiber middleware (auth, CORS, logging)
│   ├── models/             # GORM entities & data structures
│   ├── routes/             # API route definitions
│   ├── services/           # Business logic layer
│   ├── utils/              # Helper functions & utilities
│   ├── .env.example        # Environment variables template
│   └── .gitignore          # Git exclusion rules
├── frontend/               # React TypeScript Frontend
│   ├── public/             # Static assets & PWA files
│   ├── src/
│   │   ├── assets/         # Images, fonts, and visual assets
│   │   ├── components/     # Reusable UI components
│   │   │   ├── ui/         # Shadcn UI primitives
│   │   │   └── shared/     # Shared app components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── layouts/        # Page layout components
│   │   ├── lib/            # Utilities & API client
│   │   ├── pages/          # Page components
│   │   ├── services/       # API service layer
│   │   ├── store/          # Global state management
│   │   ├── types/          # TypeScript definitions
│   │   └── main.tsx        # Application entry point
│   ├── .env.example        # Frontend environment variables
│   └── .gitignore          # Git exclusion rules
└── .agent/                 # Development automation & workflows
    ├── rules/              # Coding standards & best practices
    ├── skills/             # Specialized development skills
    └── workflows/          # Step-by-step implementation guides
```

## 🛠️ Technology Stack

### Backend Technologies

- **Go 1.21+**: Modern Go programming language
- **Fiber v2**: Express-inspired web framework
- **GORM**: Full-featured ORM for Go
- **JWT**: JSON Web Token authentication
- **Bcrypt**: Secure password hashing
- **CORS**: Cross-Origin Resource Sharing
- **PostgreSQL**: Relational database

### Frontend Technologies

- **React 18+**: UI library with hooks
- **TypeScript**: Type-safe JavaScript
- **Vite 6+**: Fast build tool and dev server
- **Tailwind CSS 3**: Utility-first CSS framework
- **Shadcn UI**: Beautifully designed components
- **Zustand**: Lightweight state management
- **Axios**: HTTP client for API calls
- **Framer Motion**: Animation library
- **Lucide React**: Beautiful icons

### Development Tools

- **ESLint**: JavaScript/TypeScript linting
- **Prettier**: Code formatting
- **Golangci-lint**: Go linting
- **Hot Reload**: Fast development experience

## 🎨 Design System

### Color Palette

- **Primary**: Clean Blue/White theme
- **Accent**: Professional color scheme
- **Premium**: Google Nano Banana aesthetic

### UI Principles

- **Mobile-First**: Responsive design approach
- **Clean Minimalism**: No clutter, plenty of white space
- **Soft Geometry**: Rounded corners and smooth gradients
- **High Contrast**: Accessible color combinations
- **Professional**: Premium business appearance

## 📊 Features

### Core Functionality

- ✅ User Authentication & Authorization
- ✅ Admin Dashboard with Sidebar
- ✅ Multi-tab Interface System
- ✅ Responsive Landing Page
- ✅ Service Catalog & Pricing
- ✅ Customer Management (CRUD)
- ✅ Order/Transaction Management
- ✅ Service Management
- ✅ Data Export (CSV, XLSX, PDF)

### Advanced Features

- ✅ JWT Authentication
- ✅ Soft Delete Functionality
- ✅ Pagination & Filtering
- ✅ Search Capabilities
- ✅ Role-based Access Control
- ✅ PWA Capabilities
- ✅ Floating WhatsApp Integration
- ✅ Professional Asset Generation
- ✅ Automated Testing Workflows

## 🚀 Getting Started

### Prerequisites

- Go 1.21+ installed
- Node.js 18+ and npm
- PostgreSQL database
- Git version control

### Installation Steps

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd vibecoding-starterkit
   ```

2. **Backend Setup**

   ```bash
   cd backend
   go mod init GoClean-backend
   go mod download
   cp env.example .env
   # Configure your database and JWT settings in .env
   ```

3. **Frontend Setup**

   ```bash
   cd frontend
   npm install
   cp .env.example .env
   # Configure your API URL in .env
   ```

4. **Database Setup**
   - Create a PostgreSQL database
   - Update backend/.env with database credentials
   - Run database migrations (auto-handled by GORM)

5. **Run the Applications**

   ```bash
   # Backend (port 8080)
   cd backend && go run cmd/main.go

   # Frontend (port 5173)
   cd frontend && npm run dev
   ```

## 📋 Development Workflows

The project includes comprehensive development workflows:

1. **Backend Setup** - Initialize Go Fiber with authentication
2. **Frontend Landing Page** - Create responsive landing page
3. **Admin Dashboard Integration** - Build admin interface
4. **Testing & Debugging** - End-to-end testing procedures
5. **User Management** - Complete CRUD operations
6. **Deployment** - Railway deployment configuration
7. **Documentation** - Maintenance and updates
8. **Testing Playground** - Comprehensive testing suite

## 🎭 Agent Skills

The project includes specialized AI agent skills for:

- **Backend Development**: Go Fiber & GORM expertise
- **Frontend Development**: React & Tailwind implementation
- **CRUD Generation**: Automated module creation
- **Asset Generation**: Premium visual asset creation
- **Git Management**: Version control automation
- **App Runner**: Application execution management
- **Documentation**: Comprehensive documentation support
- **Backend Security**: Security best practices

## 🔧 Configuration

### Environment Variables

**Backend (.env)**

```env
SERVER_PORT=8090
DB_HOST=localhost
DB_PORT=5432
DB_USER=your_username
DB_PASSWORD=your_password
DB_NAME=GoClean_db
JWT_SECRET=your_jwt_secret
JWT_EXPIRY=48h
CORS_ALLOWED_ORIGINS=http://localhost:5173
APP_ENV=development
```

**Frontend (.env)**

```env
VITE_API_URL=http://localhost:8080/api
```

## 📊 API Structure

The backend follows RESTful principles with consistent response format:

```json
{
  "status": "success",
  "message": "Operation completed",
  "data": {}
}
```

### Key Endpoints

- `POST /api/auth/login` - User authentication
- `GET /api/users` - User management (with pagination)
- `POST /api/users` - Create new user
- `GET /api/services` - Service catalog
- `POST /api/orders` - Order creation

## 🧪 Testing

The project includes comprehensive testing strategies:

- **Browser Testing**: End-to-end user flow validation
- **API Testing**: Backend endpoint verification
- **UI Testing**: Component interaction testing
- **Integration Testing**: Full system validation

### Test Credentials

```
Email: admin@GoClean.com
Password: admin123
```

## 🚢 Deployment

The project is configured for deployment on Railway with:

- **Docker Support**: Containerized deployment
- **Environment Management**: Production configuration
- **Database Provisioning**: PostgreSQL setup
- **Build Optimization**: Production-ready builds

### Deployment Steps

1. Configure production environment variables
2. Build Docker containers
3. Deploy to Railway or preferred platform
4. Set up production database
5. Configure domain and SSL

## 📈 Project Status

This is a **starter template** project designed for:

- ✅ Learning full-stack development
- ✅ Rapid prototyping
- ✅ Production-ready foundation
- ✅ Customization and extension

## 🤝 Contributing

When contributing to this project:

1. Follow the established coding standards
2. Use the provided agent workflows
3. Maintain comprehensive documentation
4. Test all changes thoroughly
5. Follow the Git commit conventions

## 📝 License

This project is designed for educational and commercial use. Please review the license terms before deployment.

## 🆘 Support

For issues and questions:

1. Check the existing documentation
2. Review the agent workflows
3. Examine the code standards
4. Test with the provided workflows

---

**Built with ❤️ using modern web technologies and best practices**
