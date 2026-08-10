# 🧾 Bakery POS & Business Management System

A full-stack **Point of Sale (POS) and Business Management System** designed for bakery operations.

The system is being developed as a real-world business application covering sales, product management, customers, promotions, payments, refunds, exchanges, cashier shifts, cash drawer management, reporting, and data visualization.

> 🚧 **Project Status:** Actively under development  
> 📅 **Development:** April 2026 – Present

---

## 🚀 Overview

The Bakery POS is designed to provide a complete workflow from **product selection and sales** to **cashier management, refunds, reporting, and business analytics**.

The system supports both **USD and Lebanese Pound (LBP)** transactions and provides multilingual support for **English and Arabic**, including RTL layouts.

The application is currently being developed as a web-based system and is being prepared for deployment as a **desktop application using Electron**.

---

# 🛠️ Technology Stack

### Frontend

- Vue.js
- Vite
- Vuetify
- Pinia
- Vue Router
- Vue I18n
- HTML / CSS / JavaScript

### Backend

- Node.js
- Express.js
- REST API
- MySQL

### Desktop

- Electron
- Electron + Vue/Vite integration
- Local desktop deployment

### Data & Business Logic

- MySQL relational database
- Transaction management
- Multi-currency calculations
- Cash reconciliation
- Business reporting
- Data visualization

---

# 🛒 POS Sales

![POS Sales](screenshots/pos-sales.png)

The main POS interface used by cashiers to process customer orders.

### Features

- Product browsing by category and subcategory
- Product variants
- Sizes
- Dough options
- Shopping cart management
- Customer selection
- Quantity management
- Product options
- Discounts
- Promotions
- USD / LBP payments
- Payment calculations
- Change calculations
- Order creation
- Payment processing
- Receipt workflow

The interface is designed for fast cashier interaction while maintaining a clear overview of the current order.

---

# 🎁 Promotions Management

![Promotions](screenshots/promotions.png)

The promotions module allows administrators to create and manage promotional campaigns.

### Supported Promotion Types

- Percentage discounts
- Fixed-value discounts
- BOGO — Buy One Get One
- Bundle promotions

### Promotion Management

- Create promotions
- Edit promotions
- Activate / deactivate promotions
- Start and end dates
- Promotion priority
- Global promotions
- Customer-group promotions
- Customer-specific promotions
- Budget limits
- Promotion usage tracking

The promotion engine is designed to keep promotional rules separate from the main sales workflow.

---

# 📦 Product Management

![Product Management](screenshots/products.png)

The product management system provides administrators with tools to manage the bakery catalog.

### Features

- Products
- Categories
- Subcategories
- Product groups
- Product variants
- Sizes
- Dough options
- Units
- Product pricing
- Product configuration

The product structure is relational, allowing different product groups to support different combinations of sizes, dough types, variants, and units.

---

# 👥 Customer Management

![Customer Management](screenshots/customers.png)

The customer management module allows administrators to manage customer information and customer groups.

### Features

- Customer profiles
- Customer codes
- Contact information
- Customer groups
- VIP customers
- Family customers
- Staff customers
- Regular customers
- Customer-specific promotions
- Customer history

Customer groups can also be used by the promotion system to apply targeted offers.

---

# 💱 Refund & Exchange Management

![Refund and Exchange](screenshots/refunds-exchanges.png)

The refund and exchange module handles post-sale transactions while maintaining the original order history.

### Features

- Select items for return
- Partial refunds
- Product exchanges
- Replacement products
- Exchange balance calculations
- Returned quantities
- Exchange tracking
- Refund tracking
- Prevention of duplicate refunds
- Prevention of duplicate exchanges

The system keeps the original sale intact and records refund/exchange operations separately for better transaction tracking.

---

# 💵 Cash Drawer Management

![Cash Drawer](screenshots/cash-drawer.png)

The cash drawer module tracks physical cash handled by each cashier.

### Features

- Opening cash
- USD cash
- LBP cash
- Cash-in transactions
- Cash-out transactions
- Expected cash calculation
- Closing cash
- Cash variance
- Cashier-specific transactions

The system automatically calculates the expected drawer balance based on:

```text
Opening Cash
+ Sales
+ Cash In
- Refunds / Returns
- Cash Out
= Expected Cash