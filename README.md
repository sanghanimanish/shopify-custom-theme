# Shopify Custom Theme Development Project

## 📌 Project Overview
This project is a custom Shopify theme built on top of the Dawn theme.  
The goal of this project was to implement advanced theme customization using Liquid, metafields, AJAX cart functionality, and dynamic product rendering.

The project demonstrates backend theme logic, Shopify Liquid expertise, and frontend dynamic behavior.

---

## 🚀 Features Implemented

### 1️⃣ Custom Hero Section (Dynamic Liquid Section)

A fully customizable hero section created using Shopify Liquid.

#### Functionalities:
- Dynamic heading (editable from Theme Customizer)
- Dynamic subtext
- Custom button text and URL
- Image upload option from theme settings
- Fully responsive layout

#### Technical Implementation:
- Created a new section file: `sections/custom-hero.liquid`
- Used `schema` settings for dynamic fields
- Implemented conditional rendering for button display
- Optimized image rendering using Shopify image filters

---

### 2️⃣ Custom Product Grid Section

A dynamic product listing section with filtering and limit control.

#### Functionalities:
- Admin-controlled product limit
- Collection-based filtering
- Dynamic price display
- Sale price support (compare_at_price logic)
- Responsive product grid layout

#### Technical Implementation:
- Used `collection.products` loop
- Implemented limit control using section settings
- Used Liquid conditional statements for sale pricing
- Added collection selector inside schema settings
- Clean reusable card structure using snippets

---

### 3️⃣ Shopify Metafields Integration

Implemented custom product metafields to extend product information.

#### Functionalities:
- Created custom metafield: "Material"
- Displayed metafield dynamically on product page
- Fallback handling if metafield is empty

#### Technical Implementation:
- Used Shopify custom metafield definitions
- Accessed metafield using:
  `product.metafields.custom.material`
- Conditional rendering to prevent empty output
- Structured layout for additional product information

---

### 4️⃣ AJAX Add to Cart Functionality

Implemented asynchronous add-to-cart functionality without page reload.

#### Functionalities:
- Add to cart without refreshing page
- Dynamic cart count update
- Success and error handling
- Variant support

#### Technical Implementation:
- Used Shopify AJAX Cart API (`/cart/add.js`)
- JavaScript fetch API for POST request
- JSON payload for variant ID and quantity
- DOM manipulation for cart count update
- Error handling with try-catch

---

## 🛠 Tech Stack

- Shopify Liquid
- HTML5
- CSS3
- JavaScript (ES6)
- Shopify AJAX API
- Shopify Metafields

---

## 📂 Project Structure

- sections/
  - custom-hero.liquid
  - custom-product-grid.liquid
- snippets/
  - product-card.liquid
- assets/
  - custom.js
  - custom.css
- templates/
  - product.json

---

## 🧠 Key Learnings

- Advanced Shopify Liquid logic
- Shopify theme architecture
- AJAX-based cart handling
- Metafield integration
- Clean reusable component structure
- Performance optimization using Liquid filters

---

## 📸 Screenshots

(Add screenshots of Hero Section, Product Grid, Product Metafield Display, and AJAX Cart Working)

---

## 📌 Conclusion

This project demonstrates strong backend theme customization skills in Shopify, including Liquid development, dynamic rendering, metafield integration, and AJAX-based cart logic.

It reflects practical Shopify development experience suitable for real-world e-commerce implementations.
