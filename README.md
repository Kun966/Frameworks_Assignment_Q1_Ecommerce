# 🛒 E-commerce Database Schema (MySQL)

This repository contains a **relational database schema** for a simple E-commerce Store built with **MySQL**.  

## 📌 Features
- Customers can place multiple orders
- Products are grouped into categories
- Orders can contain multiple products (Many-to-Many)
- Payments linked One-to-One with Orders
- Includes constraints for data integrity (PK, FK, UNIQUE, NOT NULL)

## 📂 Database Schema Overview
Entities:
- **Customers**
- **Categories**
- **Products**
- **Orders**
- **Order_Items** (bridge table)
- **Payments**

### 🔗 Relationships
- One-to-Many → Customers → Orders
- One-to-Many → Categories → Products
- Many-to-Many → Orders ↔ Products (via `order_items`)
- One-to-One → Orders → Payments

## 🚀 Setup Instructions
1. Install [MySQL](https://dev.mysql.com/downloads/).
2. Clone this repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/Frameworks_Assignment_Q1_Ecommerce.git
   cd Frameworks_Assignment_Q1_Ecommerce
