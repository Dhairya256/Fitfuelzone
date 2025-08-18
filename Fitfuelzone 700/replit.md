# Overview

FitFuelZone is a beginner-friendly fitness platform that combines workouts, nutrition guidance, and daily motivation. The application features a React frontend with Express backend, focusing on accessibility and user engagement for those starting their fitness journey. The platform includes workout plans, vegetarian meal recommendations, motivational content, and a contact system for user inquiries.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React with TypeScript and Vite for fast development and building
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query for server state management and caching
- **UI Framework**: Shadcn/ui components built on Radix UI primitives with Tailwind CSS
- **Build System**: Vite with hot module replacement and development optimizations

## Backend Architecture
- **Server Framework**: Express.js with TypeScript for REST API endpoints
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Storage Layer**: Abstracted storage interface with in-memory implementation for development
- **Session Management**: Express sessions with PostgreSQL session store via connect-pg-simple
- **Development Server**: Integrated Vite middleware for seamless full-stack development

## Data Layer
- **ORM**: Drizzle ORM with PostgreSQL dialect for database schema and queries
- **Schema**: Shared TypeScript types between frontend and backend using Zod validation
- **Database Tables**: Users table for authentication, contacts table for form submissions
- **Migrations**: Drizzle migrations system for database schema management

## Authentication & Authorization
- **Session-based Authentication**: Express sessions stored in PostgreSQL
- **Form Validation**: Zod schemas for client and server-side validation
- **Contact Management**: Secure contact form submission with data persistence

## Styling & UI
- **CSS Framework**: Tailwind CSS with custom design system and CSS variables
- **Component Library**: Comprehensive Shadcn/ui component system with consistent theming
- **Design System**: Custom color palette with primary (blue), secondary (green), and accent (cyan) colors
- **Responsive Design**: Mobile-first approach with breakpoint-based responsive layouts
- **Typography**: Inter font family for modern, readable typography

## Development Tools
- **Type Safety**: Full TypeScript coverage across frontend, backend, and shared modules
- **Code Quality**: ESM modules with strict TypeScript configuration
- **Path Aliases**: Convenient import paths for components, utilities, and shared code
- **Development Experience**: Hot reload, error overlay, and development banner integration

# External Dependencies

## Database & Storage
- **Neon Database**: Serverless PostgreSQL database via @neondatabase/serverless
- **Session Store**: connect-pg-simple for PostgreSQL-backed Express sessions

## UI & Component Libraries
- **Radix UI**: Comprehensive set of accessible, unstyled UI primitives
- **Tailwind CSS**: Utility-first CSS framework with custom configuration
- **Embla Carousel**: Lightweight carousel component for content display
- **Lucide React**: Modern icon library with consistent styling

## Development & Build Tools
- **Vite**: Fast build tool with development server and hot module replacement
- **PostCSS**: CSS processing with Autoprefixer for browser compatibility
- **ESBuild**: Fast JavaScript bundler for production builds

## Validation & Forms
- **Zod**: TypeScript-first schema validation library
- **React Hook Form**: Performant forms with easy validation integration
- **Drizzle Zod**: Integration between Drizzle ORM and Zod for type-safe schemas

## State Management & API
- **TanStack Query**: Powerful data synchronization for React applications
- **Wouter**: Minimalist routing library for React applications

## Utility Libraries
- **date-fns**: Modern JavaScript date utility library
- **clsx & tailwind-merge**: Conditional class name utilities for dynamic styling
- **class-variance-authority**: Type-safe variant API for component styling