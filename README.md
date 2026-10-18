# Oak — Library Management System

Oak is a full-stack library management platform that has successfully transitioned from a legacy local desktop application built with JavaFX and OCSF (Object Client-Server Framework) to a modern, cloud-hosted web architecture. It streamlines book inventory, borrowing workflows, member tracking, waitlists, and librarian administrative operations.

🌐 **Live Application:** [https://oak-library-management-system.vercel.app](https://oak-library-management-system.vercel.app)

---

## Key Features

### Catalog & Discovery
- **Library Explorer & Search:** Browse books by title, author, ID, or subject/genre.
- **Trending & Recommendations:** Discover popular books and new arrivals.
- **Detailed Book Views:** Real-time stock availability, copy status, and description details.

### Member Portal
- **Authentication & Profiles:** Secure login and personalized member dashboard.
- **My Books:** Track currently borrowed books, due dates, borrow history, and activity logs.
- **Waitlists & Orders:** Place orders and join waitlists for checked-out titles.

### Librarian Operations
- **Borrow & Return Management:** Streamlined workflow for issuing books and processing returns.
- **Member Management:** Register new members, view and update member status, and manage account details.
- **Invoices & Communications:** Manage and track member inquiries, system notifications, and account messages.
- **Reporting & Analytics:** Advanced visual reports and charts (Recharts) tracking library metrics, borrowing trends, and inventory statistics.

---

## Architecture & Tech Stack

### Frontend (`/frontend`)
- **Framework:** React 19 with TypeScript & Vite
- **Styling:** Tailwind CSS, PostCSS
- **Routing & Visualization:** React Router DOM, Recharts
- **Hosting:** Vercel ([oak-library-management-system.vercel.app](https://oak-library-management-system.vercel.app))

### Backend (`/src/main/java`)
- **Framework:** Spring Boot 3 (Java 17) with Jakarta EE (Mail, Activation)
- **API:** RESTful architecture with JSON mapping (Jackson)
- **Build Tool:** Maven
- **Hosting:** Render Cloud Services

### Database
- **Database Engine:** MySQL 8
- **Cloud Provider:** Aiven Managed Database

---

## Local Development & Setup

### Prerequisites
- Java 17+ & Maven
- Node.js (v18+) & npm
- MySQL 8 compatible database

### 1. Database Configuration
Configure your MySQL connection properties in `src/main/resources/` or environment variables pointing to your database instance (e.g., Aiven).

### 2. Run Backend
```bash
mvn clean spring-boot:run
```

### 3. Run Frontend
```cd frontend
npm install
npm run dev
```
