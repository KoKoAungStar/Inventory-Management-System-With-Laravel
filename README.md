<p align="center"><a href="https://www.udemy.com/certificate/UC-063826cf-bd9e-481e-abea-569978113444/" target="_blank"><img src="https://udemy-certificate.s3.amazonaws.com/image/UC-063826cf-bd9e-481e-abea-569978113444.jpg?v=1687969871000" width="400"></a></p>

# 📦 Inventory Management System

A full-featured Point of Sale (POS) and Inventory Management web application built with **Laravel 9** and **PHP 8**.

---

## 🖥️ Tech Stack

| Layer | Technology |
|---|---|
| Backend Framework | Laravel 9.2 |
| Language | PHP 8.0+ |
| Frontend | Blade Templates + Tailwind CSS |
| Database | MySQL |
| Authentication | Laravel Breeze |
| Image Handling | Intervention/Image |
| PDF Export | Built-in PDF generation |
| API Client | Guzzle HTTP |

---

## ✨ Features

### 🏪 Product & Inventory
- Product management with categories, units, and images
- Real-time stock tracking and stock report (PDF export)
- Supplier-wise and product-wise stock reports

### 🛒 Purchase Management
- Record purchases from suppliers
- Purchase approval workflow (pending → approved)
- Daily purchase reports with PDF export

### 🧾 Invoice & Sales
- Create sales invoices with multiple products
- Invoice approval workflow
- Print individual invoices as PDF
- Daily invoice reports with PDF export

### 👥 Customer Management
- Full customer CRUD
- Credit customer tracking
- Paid customer tracking
- Customer-wise sales reports (credit / paid / all)
- Invoice editing and detailed view per customer

### 🏭 Supplier Management
- Full supplier CRUD
- Supplier-wise stock reports

### 📊 Reports
- Daily purchase report (PDF)
- Daily invoice/sales report (PDF)
- Stock report (PDF)
- Supplier-wise stock report (PDF)
- Product-wise stock report (PDF)
- Customer credit/paid reports (PDF)

### 🔐 Authentication
- Secure login / logout
- User profile management with image upload
- Password change functionality

---

## 🗄️ Database Schema

| Table | Description |
|---|---|
| users | Admin authentication |
| suppliers | Supplier records |
| customers | Customer records |
| categories | Product categories |
| units | Units of measurement |
| products | Product catalog with stock |
| purchases | Purchase records from suppliers |
| invoices | Sales invoice headers |
| invoice_details | Line items per invoice |
| payments | Payment records |
| payment_details | Payment breakdown details |

---

## ⚙️ Installation

### Requirements
- PHP >= 8.0
- Composer
- MySQL
- Node.js & NPM

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/KoKoAungStar/Inventory-Management-System-With-Laravel.git
cd Inventory-Management-System-With-Laravel
```

**2. Install PHP dependencies**
```bash
composer install
```

**3. Install Node dependencies**
```bash
npm install && npm run dev
```

**4. Set up environment**
```bash
cp .env.example .env
php artisan key:generate
```

**5. Configure database in `.env`**
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=inventory_db
DB_USERNAME=root
DB_PASSWORD=your_password
```

**6. Run migrations**
```bash
php artisan migrate
```

**7. Start the server**
```bash
php artisan serve
```

Visit `http://localhost:8000`

---

## 📁 Project Structure

```
app/
├── Http/Controllers/
│   ├── Pos/
│   │   ├── SupplierController.php
│   │   ├── CustomerController.php
│   │   ├── ProductController.php
│   │   ├── PurchaseController.php
│   │   ├── InvoiceController.php
│   │   ├── StockController.php
│   │   ├── CategoryController.php
│   │   └── UnitController.php
│   └── AdminController.php
├── Models/
│   ├── Supplier.php
│   ├── Customer.php
│   ├── Product.php
│   ├── Purchase.php
│   ├── Invoice.php
│   ├── InvoiceDetail.php
│   ├── Payment.php
│   └── PaymentDetail.php
database/
└── migrations/         # 14 migration files
```

---

## 🔑 Default Login

After migration, register via the registration page or seed the database.

---

## 📌 Key Concepts Demonstrated

- MVC architecture with Laravel
- Eloquent ORM relationships
- Route grouping with middleware
- Authentication with Laravel Breeze
- PDF generation for business reports
- Image upload and management
- CRUD operations across 8+ modules
- Approval workflows (Purchase & Invoice)

---

## 👨‍💻 Developer

**Ko Ko Aung**
- GitHub: [KoKoAungStar](https://github.com/KoKoAungStar)
- LinkedIn: [ko-ko-aung-dev](https://linkedin.com/in/ko-ko-aung-dev)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
