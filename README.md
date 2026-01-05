# Pet-Adoption-Management-System

# Overview
Animal shelters often struggle to manage pets, adoption requests, and user data efficiently.
This system provides a digital platform to keep track of pets, manage adoptions, and maintain a smooth workflow for shelters, ensuring every pet finds a loving home.

# Objectives

-Streamline pet management in shelters

-Facilitate pet adoption processes efficiently

-Maintain records of pets, users, and adoption requests

-Provide a user-friendly interface for shelter staff and adopters

# Features

🐶 Add, update, and manage pet information

🐾 Track adoption requests and approvals

👤 User management for adopters and staff

📄 Maintain adoption history and records

🔍 Search pets by type, age, or breed

🌐 Responsive web interface

# Tech Stack

Frontend Framework:  
React 18 - Latest React with concurrent features
TypeScript - Type-safe development
React Router v6 - Modern routing solution

UI Components:
Material-UI v5 - Complete component library
@mui/x-data-grid- Advanced data table functionality
mui/x-date-pickers - Date/time selection components
Material Icons - Comprehensive icon set

Data Visualization:
Recharts - Responsive chart library
Interactive Charts- Pie, bar, line, area charts
Real-time Updates - Live data visualization

State Management:
React Hooks- useState, useEffect, custom hooks
Context API - Global state management with AuthContext
Axios- HTTP client for API communication
Authentication State- Centralized auth management across components

Development Tools:
Create React App- Zero-config build setup
ESLint - Code quality enforcement
Prettier- Code formatting
TypeScript- Static type checking

# Installation & Setup

## Prerequisites
- Node.js 16+ 
- npm or yarn
- Backend API server running

## Installation Steps

1. **Install Dependencies**
```bash
cd frontend
npm install
```

2. **Environment Configuration**
```bash
# Create .env file
REACT_APP_API_URL=http://localhost:3001/api
```

3. **Start Development Server**
```bash
npm start
```

4. **Build for Production**
```bash
npm run build
```

# Authentication

The system includes role-based authentication with two user types:

## Admin Login
- **Username**: `admin`
- **Password**: `admin`
- **Access**: Full system access including pet management, adoption workflow, veterinary records, shelter management, and reports

## User Login
- **Username**: `user`
- **Password**: `user`
- **Access**: Limited access to view pets, adopter profiles, and submit adoption applications

## Features by Role

**Admin Capabilities:**
- Add, edit, and delete pets
- Manage adopter records
- Process adoption applications
- Access veterinary records
- Manage shelter operations
- Generate reports and analytics

**User Capabilities:**
- Browse available pets
- View adopter profiles
- Submit adoption applications
- View pet details

**Security Features:**
- Session-based authentication with localStorage persistence
- Role-based access control with dynamic UI adaptation
- Protected routes with automatic redirection
- Secure logout with complete session cleanup
- Input validation and error handling
- Professional login interface with demo credentials

  # Project Structure

```
frontend/
├── public/
│   └── index.html
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── Navbar.tsx       # Navigation with role-based menu
│   │   ├── Login.tsx        # Authentication interface
│   │   ├── ProtectedRoute.tsx # Route protection component
│   │   ├── StatCard.tsx
│   │   ├── EnhancedDashboard.tsx
│   │   ├── EnhancedPetCard.tsx
│   │   ├── PetMatchingSystem.tsx
│   │   ├── CertificateGenerator.tsx
│   │   └── NotificationSystem.tsx
│   ├── contexts/           # React Context providers
│   │   └── AuthContext.tsx  # Authentication state management
│   ├── pages/              # Main application pages
│   │   ├── Dashboard.tsx
│   │   ├── PetManagement.tsx      # Role-based pet operations
│   │   ├── EnhancedPetManagement.tsx
│   │   ├── AdopterManagement.tsx  # Role-based adopter management
│   │   ├── AdoptionWorkflow.tsx   # Admin-only workflow
│   │   ├── VeterinaryRecords.tsx  # Admin-only vet records
│   │   ├── ShelterManagement.tsx  # Admin-only shelter ops
│   │   └── Reports.tsx            # Admin-only analytics
│   ├── services/           # API service layer
│   │   └── apiService.ts    # Enhanced with mock data
│   ├── types/              # TypeScript type definitions
│   │   └── index.ts
│   ├── utils/              # Utility functions
│   ├── App.tsx             # Main app with auth provider
│   └── index.tsx           # Application entry point
├── package.json
└── README.md
```

# System Workflow

Shelter staff (ADMIN) adds new pets into the system

Users browse available pets

Users submit adoption requests

Staff reviews and approves adoption requests

System updates pet status and maintains adoption records


# Database Integration

The system includes a comprehensive MySQL database with:

## Database Schema
- **26 Pets** - Dogs, Cats, Birds, Rabbits, Fish, Hedgehogs, Guinea Pigs, Ferrets, Pigs
- **6 Shelters** - Multiple locations with capacity tracking
- **10 Adopters** - Diverse profiles with different species preferences
- **25 Adoption Records** - Complete application workflow tracking
- **41 Veterinary Records** - Comprehensive medical history and care
- **Stored Procedures** - Full CRUD operations for all entities

## Data Features
- **Multi-year Data** - 2022-2024 adoption statistics and trends
- **Species Diversity** - 9 different animal species with specialized care
- **Realistic Data** - Professional mock data for demonstration
- **Comprehensive Records** - Medical, adoption, and shelter management data

This frontend provides a complete, professional interface for managing all aspects of pet adoption operations with modern web technologies, secure authentication, and comprehensive data management.

# Learning Outcomes

-Built a full-stack web application

-Gained experience in user management and database operations

-Practiced frontend-backend integration

# Future Enhancements

-Add notifications for adoption requests

-Integrate AI-based pet recommendation for adopters

-Implement role-based access control

-Deploy as a live web application
