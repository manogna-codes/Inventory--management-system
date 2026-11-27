# Inventory--management-system
# 📦 Inventory Management System

### A Secure, Role-Based Web Application for Product, Stock and Sales Management

## 📌 Project Overview

The **Inventory Management System** is a secure, responsive, browser-based web application developed to simplify and automate inventory management operations.

The system provides a centralized platform to manage products, categories, warehouse stock, sales transactions and user activities. It helps reduce manual record-keeping errors, monitor stock availability, identify low-stock products and maintain accurate inventory records.

The application uses role-based access control to ensure that users can access features according to their assigned permissions.

## 🎯 Project Objectives

- Develop a centralized inventory management platform.
- Manage products, categories and stock quantities.
- Monitor warehouse inventory and low-stock alerts.
- Simplify sales transactions through a Point of Sale (POS) system.
- Maintain stock-in, stock-out and adjustment records.
- Implement secure authentication and role-based authorization.
- Provide dashboard analytics for inventory monitoring.

## ✨ Key Features

### 1. User Authentication
- User registration and login.
- Secure password hashing.
- Session management using JSON Web Tokens.
- Protected application routes.
- Password change and profile management.

### 2. Dashboard
- Total product statistics.
- Low-stock alerts.
- Inventory value calculation.
- Seven-day sales trend.
- Category-wise stock value.
- Recent inventory activity.

### 3. Product Management
- Add new products.
- Edit existing product details.
- Delete products.
- Search products by SKU, name or category.
- Manage supplier details, quantity and unit price.

### 4. Category Management
- Create product categories.
- Update category details.
- Search and manage categories.
- Prevent deletion of categories that are still associated with products.

### 5. Warehouse Management
- Monitor available stock.
- View total inventory quantities.
- Identify products requiring restocking.
- Display stock status based on reorder levels.

### 6. Point of Sale (POS)
- Select products for sales.
- Enter product quantities.
- Automatically calculate invoice totals.
- Validate stock availability before completing sales.
- Automatically update inventory after successful transactions.

### 7. Stock Movement Tracking
- Record stock-in operations.
- Record stock-out operations.
- Record inventory adjustments.
- Maintain movement history with timestamps and responsible users.

### 8. User Administration
- View registered users.
- Manage user roles.
- Activate or deactivate accounts.
- Restrict administrative operations to authorized users.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| React 19 | Frontend development |
| TypeScript | Type-safe programming |
| Express.js | Backend server |
| tRPC | Frontend-backend communication |
| MySQL | Database management |
| Drizzle ORM | Database operations |
| Zod | Input validation |
| Wouter | Client-side routing |
| Vite | Development and build tool |
| Tailwind CSS | User interface styling |
| Vitest | Automated testing |
| pnpm | Package management |

## 🏗️ System Architecture

The application follows a three-layer architecture:

**1. Presentation Layer**
- React
- TypeScript
- Frontend components
- User interface

**2. Application Layer**
- Express.js
- tRPC routers
- Authentication
- Business logic
- Input validation

**3. Data Layer**
- MySQL
- Drizzle ORM
- Database schemas
- Database transactions

## 🗄️ Database Design

The application uses MySQL with four principal database tables:

| Table | Description |
|---|---|
| Users | Stores user accounts, roles and authentication details. |
| Categories | Stores product category information. |
| Products | Stores product details, quantities and pricing. |
| Stock Movements | Maintains stock-in, stock-out and adjustment records. |

## 🔐 Security Features

- Password hashing using Node.js scrypt.
- Signed JSON Web Tokens.
- HTTP-only session cookies.
- Role-based access control.
- Server-side authorization.
- Zod input validation.
- Rate limiting for registration and login attempts.
- Protection against unauthorized operations.

## 👥 User Roles

The application supports three user roles:

| Role | Permissions |
|---|---|
| Administrator | Complete system access, including user management. |
| Manager | Product, category, warehouse and inventory management. |
| Staff | View inventory, create POS sales and manage personal profiles. |

## ⚙️ Installation and Setup

### Prerequisites

Make sure the following tools are installed:

- Node.js
- pnpm
- MySQL
- Git

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

### Step 2: Navigate to the Project Directory

```bash
cd College_project_2026
```

### Step 3: Configure Environment Variables

Create an environment file:

```powershell
Copy-Item .env.example .env
```

Configure the following variables in the `.env` file:

```env
DATABASE_URL=your_mysql_database_url
JWT_SECRET=your_secure_random_secret
```

### Step 4: Install Dependencies

```bash
pnpm install
```

### Step 5: Apply Database Migrations

```bash
pnpm db:migrate
```

### Step 6: Start the Development Server

```bash
pnpm dev
```

### Step 7: Open the Application

Open the following address in your browser:

```text
http://localhost:3000/inventory-management
```

**Note:** The MySQL database must be configured and accessible before running the application. The first registered account receives Administrator privileges.

## 🧪 Testing

The project includes automated tests using Vitest.

Run the following commands:

**TypeScript Validation**
```bash
pnpm check
```

**Run Automated Tests**
```bash
pnpm test
```

**Production Build**
```bash
pnpm build
```

The project report records 14 automated tests passing, zero TypeScript errors and a successful production build.

## 🎥 Project Video Presentation

**Video Demonstration:**  
[Insert Google Drive Video Link Here]

The video presentation demonstrates the application's features, workflow, inventory operations, dashboard and POS functionality.

## 📄 Project Report

The complete project documentation is available in this repository.

**Project Report:** `Inventory_Management_System_Report.pdf`

## 👨‍💻 Team Members

This project was developed collaboratively by six students of B.Tech Computer Science and Engineering, Section O, SRM University-AP.

| Student Name | Registration Number |
|---|---|
| M. Manogna | AP24110011731 |
| M. Kirthika | AP24110011090 |
| K. Yasaswi | AP24110011744 |
| D. Lokasree Ranga Priya | AP24110010619 |
| P. Karthik | AP24110010659 |
| K. Bhagya Sri Kota | AP24110010150 |

**Project Guide:** Mr. Bala Venkateswarlu

**University:** SRM University-AP  
**Department:** Computer Science and Engineering  
**Academic Year:** 2026–2027

## 🚀 Future Enhancements

- Email-based password reset functionality.
- CSV and Excel report exports.
- Automatic low-stock email notifications.
- Barcode scanning.
- Multi-item invoices.
- Downloadable PDF receipts.
- Advanced sales and inventory reports.

## 📝 Conclusion

The Inventory Management System provides an integrated solution for managing products, stock, warehouse operations, sales and user activities.

By combining modern frontend technologies, backend APIs, database management and security mechanisms, the application demonstrates the practical implementation of full-stack web development concepts.

The project aims to improve inventory accuracy, operational efficiency, security and accountability through a centralized management platform.

---

**Developed as an Academic Project | SRM University-AP | 2026–2027**
