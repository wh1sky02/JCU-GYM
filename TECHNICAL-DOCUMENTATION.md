# JCU Gym Management System - Technical Documentation

## 1. Project Overview

The JCU Gym Management System is a full-stack web application built for managing a university gym facility. It provides features for session booking, user management, attendance tracking, and administrative oversight. The system is designed to handle multiple user roles (students and administrators) with different access levels and capabilities.

### Core Features
- User authentication and authorization
- Session booking and management
- Attendance tracking
- Administrative dashboard with analytics
- Real-time booking availability
- Automated waitlist management
- User notifications
- Billing and payment tracking

## 2. Technical Stack

### Frontend
- **Next.js 15.2.4 (App Router)**
  - Server-side rendering
  - API routes integration
  - Advanced routing with layout system
  - Built on React 19

- **React 19**
  - Server and client components
  - Hooks for state management
  - Component composition

- **TypeScript 5**
  - Static typing
  - Interface definitions
  - Type safety across the application

- **UI Framework**
  - Tailwind CSS 3.4.17 for styling
  - shadcn/ui components (based on Radix UI)
  - Lucide React for icons
  - Custom UI components in `/components/ui`

- **Form Handling**
  - React Hook Form with Zod validation
  - Custom form components and hooks
  - Client-side validation patterns

### Backend
- **Next.js API Routes**
  - RESTful API structure in `/app/api`
  - Request validation
  - Error handling middleware

- **Database**
  - PostgreSQL (via Neon.tech)
  - Direct SQL queries using `node-postgres (pg)`
  - Connection pooling
  - Prepared statements for security

- **Authentication**
  - JWT-based authentication
  - Secure password hashing (bcryptjs)
  - Session management
  - Role-based access control

## 3. Architecture & Implementation

### Database Schema
The database uses a normalized schema with the following core tables:
\`\`\`sql
- users: User accounts and profiles
- gym_sessions: Available gym sessions
- bookings: Session bookings and attendance
- notifications: System notifications
- billing_transactions: Payment records
- user_achievements: User rewards and achievements
\`\`\`

### API Structure
\`\`\`
/api/
├── admin/
│   ├── approve-user/
│   ├── billing/
│   ├── bookings/
│   ├── sessions/
│   └── stats/
├── auth/
│   ├── login/
│   ├── logout/
│   └── register/
├── bookings/
├── notifications/
└── sessions/
\`\`\`

### Frontend Architecture
\`\`\`
/app/
├── admin/
│   ├── dashboard/
│   └── login/
├── auth/
│   ├── login/
│   └── register/
└── dashboard/
    ├── book/
    └── history/
\`\`\`

## 4. Core Functionality Implementation

### Authentication Flow
1. User registration via `/api/auth/register`
2. Admin approval required for new accounts
3. JWT token generation on successful login
4. Token validation middleware for protected routes

### Booking System
\`\`\`typescript
interface Booking {
  id: string
  userId: string
  sessionId: string
  status: "confirmed" | "cancelled" | "no-show" | "completed"
  bookingDate: string
  checkInTime?: string
  checkOutTime?: string
  isRecurring: boolean
}
\`\`\`

### Database Operations
The system uses a custom database adapter pattern:
\`\`\`typescript
class CloudDatabase {
  async createBooking(bookingData: any): Promise<any>
  async getUserBookings(userId: string): Promise<Booking[]>
  async updateSessionBookingCount(sessionId: string, increment: number): Promise<void>
}
\`\`\`

## 5. Key Libraries & Tools

- **Date Handling**: date-fns for date manipulation
- **Calendar**: react-day-picker for date selection
- **Forms**: @hookform/resolvers for form validation
- **UI Components**: 
  - @radix-ui/* for accessible components
  - class-variance-authority for component variants
- **Database**: pg and pg-pool for PostgreSQL connection
- **Security**: bcryptjs and jsonwebtoken

## 6. Setup Instructions

### Development Environment
1. Install Node.js
2. Clone repository
3. Set up PostgreSQL database on Neon.tech
4. Configure environment:
\`\`\`bash
# .env.local
DATABASE_URL=postgres://[USER]:[PASSWORD]@[HOST]/[DATABASE]?sslmode=require
JWT_SECRET=your-secret-key
\`\`\`
5. Install dependencies: \`npm install\`
6. Run database setup: \`node scripts/setup-schema.js\`
7. Start development server: \`npm run dev\`

### Production Deployment
1. Build application: \`npm run build\`
2. Set production environment variables
3. Start production server: \`npm start\`

## 7. Custom Utilities & Hooks

### Custom Hooks
- \`use-mobile.tsx\`: Responsive design detection
- \`use-toast.ts\`: Toast notification system

### Utility Functions
Located in `/lib/utils.ts`:
- Database adapters
- Type conversions
- Date formatting
- Authentication helpers

## 8. Performance & Security

### Security Measures
- Password hashing with bcryptjs
- Prepared SQL statements
- JWT token validation
- Role-based access control
- Input validation with Zod

### Performance Optimizations
- Connection pooling for database
- Indexed database queries
- Server-side rendering
- Optimized PostgreSQL schema

## 9. Summary & Design Decisions

The technology stack was chosen to provide:

1. **Developer Experience**
   - TypeScript for type safety
   - Next.js for simplified deployment
   - Modern tooling and frameworks

2. **Performance**
   - Server-side rendering
   - Optimized database queries
   - Connection pooling

3. **Maintainability**
   - Clear project structure
   - Type definitions
   - Component modularity

4. **Scalability**
   - PostgreSQL for reliable data storage
   - Serverless-ready architecture
   - Modular API design

## 10. Known Limitations & Future Improvements

1. **Potential Enhancements**
   - Real-time updates using WebSockets
   - Enhanced analytics dashboard
   - Mobile application
   - Automated testing suite

2. **Current Limitations**
   - Limited payment gateway integration
   - Basic notification system
   - Manual session management

This documentation reflects the current implementation while providing insight into the system's architecture and design decisions.
