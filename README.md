# AssetFlow - Enterprise Asset & Resource Management System

A comprehensive, single-page application for managing organizational assets, resources, and maintenance workflows.

## 📋 Overview

AssetFlow is an enterprise-grade asset and resource management system designed to help organizations track, allocate, and maintain their physical assets and shared resources. Built as a single-page application with persistent storage, it provides a complete solution for asset lifecycle management.

**Live Demo:** [AssetFlow Application](https://your-demo-url.com)

## ✨ Features

### 1. 🔐 Authentication
- Email/password login
- Account creation (Employee role)
- Role-based access control
- Session management

### 2. 📊 Dashboard
- KPI cards: Assets Available, Allocated, Maintenance, Active Bookings, Overdue Returns
- Quick action buttons: Register Asset, Book Resource, Raise Maintenance
- My Assets view
- Real-time notifications

### 3. 🏢 Organization Setup (Admin Only)
- **Departments:** Create, edit, assign heads, parent-child hierarchy
- **Asset Categories:** Define categories with custom fields
- **Employee Directory:** Manage employees, promote roles (Department Head, Asset Manager)

### 4. 📦 Asset Management
- Register assets with auto-generated tags (AF-0001 format)
- Track lifecycle states: Available, Allocated, Reserved, Under Maintenance, Lost, Retired, Disposed
- Search/filter by tag, serial, category, status
- Asset history tracking
- Photo/document attachments support

### 5. 🔄 Asset Allocation
- Allocate assets to employees/departments
- Conflict prevention (can't allocate already-taken assets)
- Transfer workflow: Request → Approve → Re-allocate
- Return flow with condition check-in
- Auto-flag overdue returns

### 6. 📅 Resource Booking
- Time-slot booking for shared resources
- Overlap validation (prevents double-booking)
- Calendar view of existing bookings
- Cancel/reschedule functionality
- Reminder notifications

### 7. 🔧 Maintenance Management
- Raise maintenance requests with priority levels
- Approval workflow: Pending → Approved/Rejected → In Progress → Resolved
- Auto-update asset status to "Under Maintenance"
- Maintenance history per asset

### 8. 📋 Asset Audits
- Create audit cycles with date ranges
- Assign multiple auditors
- Mark assets: Verified / Missing / Damaged
- Auto-generate discrepancy reports
- Close audit cycles with status updates

### 9. 📈 Reports & Analytics
- Asset utilization trends
- Category-wise distribution
- Maintenance frequency analysis
- Department allocation summaries

### 10. 📝 Activity Logs
- Complete audit trail
- Who did what, when
- Filterable by user/action

## 🏗️ Architecture

### Tech Stack
- **Frontend:** Vanilla JavaScript, HTML5, CSS3
- **State Management:** In-memory store with localStorage persistence
- **Styling:** Custom CSS with CSS Variables
- **Icons:** Font Awesome 6
- **Fonts:** Inter (Google Fonts)

### Data Structure
```javascript
{
  users: [],          // Employees with roles
  departments: [],    // Org structure
  categories: [],     // Asset categories
  assets: [],         // Assets with lifecycle
  bookings: [],       // Resource bookings
  maintenance: [],    // Maintenance requests
  audits: [],         // Audit cycles
  notifications: [],  // User notifications
  logs: [],           // Activity audit trail
  currentUserId: null // Active session
}

## developed by:
Priyadharshini S
Ragavarshini G
Raguram
