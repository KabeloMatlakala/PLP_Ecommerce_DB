# 🛍️ PLP_Ecommerce Database

This repository contains the SQL schema and Entity Relationship Diagram (ERD) for **PLP_Ecommerce**, a scalable and modular database design tailored for an e-commerce platform. The design supports product management, variations, attributes, and inventory tracking for a modern product listing page (PLP) system.

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `plp_ecommerce.sql` | Full SQL script to create the database schema. Includes all tables, relationships, and constraints. |
| `plp_ecommerce_ERD.png` | PNG image of the Entity Relationship Diagram for quick visual reference. |
| `plp_ecommerce_ERD.drawio` | Editable ERD file (open with [draw.io / diagrams.net](https://app.diagrams.net)) for future modifications. |

---

## 🧠 Overview

The database schema is normalized and supports:

### ✅ Core Entities

- **Brands & Categories**: Organize products by brand and category.
- **Products**: Main product entries with base prices and metadata.
- **Variations**: Each product can have multiple size/color variations.
- **Stock Items**: Track inventory and pricing for each variant.
- **Images**: Support multiple product images.
- **Attributes**: Add custom, dynamic attributes like material, fit, or gender.

---

## 🧱 Key Tables & Relationships

- `brand`, `product_category`: Basic classification tables.
- `product`: Linked to brand & category.
- `color`, `size_option`, `size_category`: Variation dimension tables.
- `product_variation`: Links product with a unique size + color combination.
- `product_item`: Final sellable units with price and stock.
- `product_image`: Stores image URLs for products.
- `attribute_category`, `attribute_type`, `product_attribute`: Fully dynamic attribute system.

---

## 🛠️ Setup Instructions

You can set up and visualize the database using **XAMPP** or **MySQL Workbench**.

### Option 1: XAMPP (with phpMyAdmin)

1. Download & install [XAMPP](https://www.apachefriends.org/index.html)
2. Launch XAMPP Control Panel and start **Apache** and **MySQL**
3. Open **phpMyAdmin** (`http://localhost/phpmyadmin`)
4. Create a new database named `PLP_Ecommerce`
5. Import the `plp_ecommerce.sql` file into the database

### Option 2: MySQL Workbench

1. Download & install [MySQL Workbench](https://dev.mysql.com/downloads/workbench/)
2. Connect to your local MySQL Server
3. Create a new schema named `PLP_Ecommerce`
4. Open a new SQL tab, paste the contents of `plp_ecommerce.sql`, and execute
5. To view the ERD:
   - Go to **Database > Reverse Engineer**
   - Select your schema and generate the diagram

---

## 🖼️ Visualizing the ERD

For easy customization and sharing, the ERD is also provided in draw.io format:

- Open `plp_ecommerce_ERD.drawio` in [draw.io](https://app.diagrams.net)
- Or view the exported image: `plp_ecommerce_ERD.png`

---

## 👨‍💻 Author

**Kabelo Peter Matlakala**  
📍 Polokwane, South Africa  
📧 [matlakalakabelo1@gmail.com](mailto:matlakalakabelo1@gmail.com)  
🌐 [Portfolio](https://delightplus.github.io/)  
💻 [GitHub](https://github.com/KabeloMatlakala)

---

## 📄 License

This project is open for educational and commercial use. Attribution appreciated, but not required.

---
