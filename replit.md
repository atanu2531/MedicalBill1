# MedicalBill - Pharmacy Management System

## Overview

MedicalBill is a comprehensive pharmacy management application designed to streamline medical shop operations. The system provides inventory management, prescription handling, and medicine database lookup capabilities through a modern web interface. Built as a full-stack TypeScript application, it targets pharmacy owners who need efficient tools for managing their business operations.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **React with TypeScript**: Modern component-based UI using React with TypeScript for type safety
- **Wouter Router**: Lightweight routing solution for single-page application navigation
- **shadcn/ui Component Library**: Consistent design system using Radix UI primitives with Tailwind CSS styling
- **TanStack Query**: Client-side state management and data fetching with caching and synchronization
- **React Hook Form**: Form handling with validation using Zod schemas
- **Tailwind CSS**: Utility-first CSS framework with custom design tokens and responsive design

### Backend Architecture
- **Express.js Server**: RESTful API server with TypeScript support
- **Drizzle ORM**: Type-safe database operations with PostgreSQL
- **Replit Authentication**: OpenID Connect integration for user authentication and session management
- **File Upload System**: Multer-based file handling for prescription document uploads
- **Modular Route Structure**: Organized API endpoints with middleware for authentication and error handling

### Database Design
- **PostgreSQL with Drizzle**: Relational database with type-safe schema definitions
- **Core Tables**:
  - Users: Authentication and profile management
  - Medicines: Inventory tracking with stock levels and categorization
  - Prescriptions: Document storage with patient information
  - Medicine Database: Reference data for drug information lookup
  - Sessions: Secure session storage for authentication state

### Authentication & Authorization
- **Replit OpenID Connect**: Integrated authentication system with automatic user provisioning
- **Session-based Security**: Server-side session management with PostgreSQL storage
- **Protected Routes**: Middleware-based route protection with automatic redirect handling
- **User Context**: React-based authentication state management with automatic token refresh

### Data Management Patterns
- **Optimistic Updates**: Client-side state updates with server synchronization
- **Query Invalidation**: Automatic cache updates when data changes
- **Form Validation**: Zod schema validation on both client and server
- **Error Handling**: Centralized error management with user-friendly messages

### File Storage Strategy
- **Local File System**: Direct file storage for prescription uploads with organized directory structure
- **File Type Validation**: Restricted to medical document formats (PDF, JPG, PNG)
- **Size Limitations**: 10MB maximum file size with proper error handling
- **Secure Access**: Protected file serving through authenticated endpoints

### Development & Build System
- **Vite Build Tool**: Fast development server with hot module replacement
- **TypeScript Configuration**: Strict type checking with path aliases for clean imports
- **ESM Modules**: Modern JavaScript module system throughout the application
- **Development Mode**: Integrated Replit development tools with runtime error overlay

## External Dependencies

### Database Services
- **Neon PostgreSQL**: Serverless PostgreSQL database with connection pooling
- **Drizzle Kit**: Database migration and schema management tools

### Authentication Infrastructure
- **Replit OpenID Provider**: Integrated authentication service with user management
- **connect-pg-simple**: PostgreSQL session store for Express sessions

### UI Component Libraries
- **Radix UI**: Comprehensive set of accessible UI primitives
- **Lucide React**: Icon library with consistent design language
- **React Hook Form**: Form state management with validation integration

### Development Tools
- **Vite Plugins**: Development enhancement tools including error overlay and cartographer
- **ESBuild**: Fast JavaScript bundler for production builds
- **PostCSS**: CSS processing with Tailwind CSS integration

### File Processing
- **Multer**: Multipart form data handling for file uploads
- **Date-fns**: Date manipulation and formatting utilities

### Utility Libraries
- **Zod**: Runtime type validation and schema definition
- **Class Variance Authority**: Type-safe CSS class composition
- **clsx & twMerge**: Conditional CSS class management