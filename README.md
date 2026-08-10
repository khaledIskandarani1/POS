# 🧾 Bakery POS & Business Management System

A full-stack **Point of Sale (POS) and business management system** designed for bakery operations.

The system is currently under active development, with approximately **4 months of development** focused on building the sales workflow, product management, promotions, customer management, payments, cash drawer operations, refunds/exchanges, multilingual support, and business reporting.

The goal is to build a complete bakery management platform that can eventually support daily sales, cashier operations, inventory, kitchen workflows, and business analytics from a single application.

---

## 🚀 Project Overview

The system is designed around several core areas:

- 🛒 Point of Sale & Sales Management
- 📦 Product & Catalog Management
- 🎁 Promotions & Discounts
- 👥 Customer Management
- 💳 Payment Processing
- 💱 Refund & Exchange Management
- 💵 Cash Drawer Management
- 🕐 Cashier Shift Management
- 📊 Reports & Data Visualization
- 🌍 Multilingual Interface
- 🖥️ Desktop Application with Electron
- 📦 Inventory Management *(Planned)*
- 🧾 Barcode Integration *(Planned)*
- 👨‍🍳 Kitchen Management *(Planned)*

---

# 🛠️ Technology Stack

### Frontend

- Vue.js
- Vite
- Vuetify
- Pinia
- Vue Router
- Vue I18n
- JavaScript

### Backend

- Node.js
- Express.js
- REST API

### Database

- MySQL
- Relational database design

### Desktop

- Electron *(In Progress)*

---

# 🛒 POS Sales System

The POS interface is designed for fast cashier interaction while maintaining a clear overview of the current order.

### Product Browsing

Cashiers can browse products through categories and subcategories.

![POS Sales Screen](screenshots/pos/sales-screen.png)

### Product Configuration

Products can support different variants, sizes, dough types, and other configurable options.

![Product Selection](screenshots/pos/product-selection.png)

### Shopping Cart

The cart manages quantities, products, customers, discounts, and order totals.

![Shopping Cart](screenshots/pos/cart.png)

### Payment Processing

The system supports multi-currency payments using **USD and Lebanese Pounds (LBP)**.

![Payment Screen](screenshots/pos/payment.png)

### Implemented Features

- Category and subcategory browsing
- Product variants
- Sizes
- Dough options
- Shopping cart
- Quantity management
- Customer selection
- Discounts
- Promotions
- USD / LBP payments
- Order creation
- Payment processing

---

# 🎁 Promotions Management

The promotion module allows administrators to create and manage promotional campaigns without modifying the underlying sales logic.

### Promotion Management

Administrators can create, edit, activate, and deactivate promotions.

![Promotion Management](screenshots/promotions/promotion-list.png)

### Promotion Types

The system supports several promotion types:

- Percentage discounts
- Fixed-value discounts
- BOGO — Buy One Get One
- Bundle promotions

![Promotion Types](screenshots/promotions/promotion-types.png)

### Promotion Targeting

Promotions can be applied to different scopes:

- Global
- Customer groups
- Individual customers
- Product/group-based promotions

![Promotion Targeting](screenshots/promotions/promotion-settings.png)

### Promotion Scheduling

Promotions can have:

- Start dates
- End dates
- Priority
- Activation status
- Budget limits
- Usage tracking

---

# 📦 Product Management

The product management system provides administrators with a structured catalog for bakery products.

![Product Management](screenshots/products/products.png)

### Product Structure

The catalog supports:

- Products
- Categories
- Subcategories
- Product groups
- Product variants
- Sizes
- Dough options
- Units
- Pricing
- Product configuration

![Product Configuration](screenshots/products/product-composer.png)

The database uses a relational structure so that different product groups can have different combinations of sizes, dough types, variants, and units.

---

# 👥 Customer Management

The customer module allows the business to maintain customer information and organize customers into groups.

![Customer Management](screenshots/customers/customers.png)

### Features

- Customer profiles
- Customer codes
- Contact information
- Customer groups
- Customer history
- Customer-specific promotions

### Customer Groups

Example groups include:

- VIP
- Family
- Staff
- Regular

![Customer Groups](screenshots/customers/customer-groups.png)

---

# 💱 Refund & Exchange Management

The system includes workflows for handling post-sale refunds and product exchanges while maintaining the original transaction history.

![Refund Management](screenshots/refunds/refund.png)

### Refunds

- Full refunds
- Partial item refunds
- Returned quantities
- Refund tracking

### Exchanges

- Select products for exchange
- Return original products
- Select replacement products
- Calculate exchange balances
- Track exchanged quantities

![Exchange Management](screenshots/refunds/exchange.png)

The original order remains intact while refund and exchange operations are recorded separately.

---

# 💵 Cash Drawer Management

The cash drawer module tracks the physical cash handled by each cashier.

![Cash Drawer](screenshots/cash-drawer/transactions.png)

### Features

- Opening cash
- USD balance
- LBP balance
- Cash-in transactions
- Cash-out transactions
- Expected cash
- Closing cash
- Cash variance
- Cashier-specific transactions

The system calculates expected cash dynamically from:

**Opening Cash + Sales + Cash In − Cash Out − Returns**

This provides a basic reconciliation system between system-generated cash and the physical drawer.

---

# 🕐 Cashier Shift Management

Cashier shifts provide a structured lifecycle for each cashier session.

![Shift Management](screenshots/shifts/open-shift.png)

### Shift Workflow

1. Cashier opens a shift
2. Opening cash is recorded
3. Sales and drawer transactions are associated with the shift
4. Cashier closes the shift
5. Closing cash is recorded
6. Expected vs. actual cash is calculated
7. The shift becomes part of the historical record

![Shift History](screenshots/shifts/shift-history.png)

### Features

- Open shift
- Opening cash
- Cashier identification
- Shift status
- Closing cash
- Shift history
- Expected cash
- Actual closing cash
- Cash variance

---

# 📊 Shift Reports & Data Visualization

The reporting module combines transactional data from different parts of the system and transforms it into business-level information.

![Shift Reports](screenshots/reports/shift-report.png)

### Reports Include

- Shift performance
- Cash received
- Refunds
- Cash-in transactions
- Cash-out transactions
- Expected cash
- Actual closing cash
- Cash differences
- USD / LBP conversion
- Cashier performance

### Data Visualization

The reporting system is being expanded to provide visual representations of business data.

![Data Visualization](screenshots/reports/visualization.png)

Future dashboards will provide better visibility into:

- Sales trends
- Product performance
- Promotion performance
- Customer behavior
- Cashier performance
- Revenue
- Inventory levels

---

# 🌍 Multilingual Interface

The application supports multiple languages using **Vue I18n**.

![English Interface](screenshots/multilingual/english.png)

### Currently Supported

- 🇬🇧 English
- 🇱🇧 Arabic

### Features

- Dynamic language switching
- RTL support for Arabic
- Translated interface labels
- Localized messages
- Localized product information

![Arabic RTL Interface](screenshots/multilingual/arabic.png)

The goal is to make the system accessible to both English- and Arabic-speaking employees.

---

# 🖥️ Desktop Application

## Electron — In Progress

The POS is currently being prepared for deployment as a desktop application using **Electron**.

![Electron Application](screenshots/electron/desktop-app.png)

The objective is to provide a dedicated desktop POS experience while keeping the existing Vue.js frontend and Node.js backend architecture.

### Planned Electron Capabilities

- Desktop POS application
- Local application environment
- Hardware integration
- Printer integration
- Barcode scanner integration
- Offline/local operation
- Automatic application updates

---

# 🔮 Future Development

The following features are planned as the project continues to evolve.

---

## 🧾 Barcode Integration

### Planned

- Barcode scanner support
- Barcode generation
- Barcode label printing
- Product barcode assignment
- Fast barcode-based product lookup

The goal is to allow cashiers to scan products directly into the POS instead of manually searching for them.

---

## 📦 Inventory Management

### Planned

- Stock tracking
- Stock levels
- Stock movements
- Stock adjustments
- Purchase/stock entries
- Low-stock alerts
- Inventory reports
- Product stock history

Inventory will eventually be integrated directly with sales so that stock levels can be updated automatically after transactions.

---

## 👨‍🍳 Kitchen Management System

### Planned

- Kitchen order display
- New order notifications
- Order preparation status
- Preparing / Ready / Completed workflow
- Kitchen order queue
- Order prioritization
- Completed order tracking

The goal is to connect the POS directly with the bakery's kitchen workflow.

---

## 📊 Advanced Business Analytics

### Planned

The reporting system will eventually expand beyond shift reports into a complete business analytics dashboard.

Planned metrics include:

- Daily sales
- Monthly sales
- Revenue trends
- Best-selling products
- Product profitability
- Promotion performance
- Customer purchasing behavior
- Cashier performance
- Inventory performance
- Sales by category
- Sales by payment method

---

# 🔐 Security & Access Control

Future development will also expand the authentication and authorization system.

### Planned

- Role-based access control
- Admin accounts
- Cashier accounts
- Permission management
- Audit logs
- Restricted administrative operations

---

# 🏗️ Architecture

The application follows a client-server architecture:

```text
┌─────────────────────────────┐
│       Vue.js Frontend       │
│                             │
│  Vuetify · Pinia · I18n     │
└──────────────┬──────────────┘
               │
               │ REST API
               ▼
┌─────────────────────────────┐
│      Node.js / Express      │
│                             │
│ Authentication              │
│ Sales                       │
│ Payments                    │
│ Promotions                  │
│ Customers                   │
│ Shifts                      │
│ Cash Drawer                 │
│ Reports                     │
└──────────────┬──────────────┘
               │
               ▼
┌─────────────────────────────┐
│           MySQL             │
│                             │
│ Products                    │
│ Orders                      │
│ Payments                    │
│ Customers                   │
│ Promotions                  │
│ Shifts                      │
│ Transactions                │
└─────────────────────────────┘
