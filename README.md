# 🚀 MKR Enterprise ERP System

**Type**: B2B & B2C Business ERP  
**Scope**: Inventory, Sales, Purchase, Delivery, Accounts, CRM  
**Platform**: Web (React + Vite + Supabase) | Mobile App (React Native / Flutter)  
**Status**: Active Development  
**Owner**: MKR Enterprise  
**Tech Stack**: React, Tailwind, Supabase, Node, Vercel, Telegram API, WhatsApp Cloud API  

---

## 🌟 Project Highlights

- Walk-in Sales Support (No Customer Entry Required)
- Route-wise Van Load Sheet Generator (PDF/Excel)
- Auto Profit Calculation per Invoice (Non-editable)
- Cash & Bank Book with Opening Balance
- Role-based Access (Admin, Manager, Sales, Delivery, Accountant)
- Offline Data Entry with Auto Sync every 1 minute
- Telegram-based Daily/Weekly/Monthly Reporting
- WhatsApp Order/Delivery Confirmation
- Document Upload per Customer
- Internal Activity Logs for Admin Audit
- Auto Backup to Google Drive (Daily)

---

## 📦 Modules

### 🔸 Sales
- Walk-in Customer Sales (no data entry needed)
- Invoice viewable by all users
- Profit auto-calculated per invoice (no manual edits)
- Discounts visible with daily/weekly/monthly summaries via Telegram
- Minimum margin enforcement (10%)

### 🔸 Purchase
- Supplier tagging
- Product cost affects P&L and stock valuation

### 🔸 Inventory
- FIFO valuation
- Dead Stock & Slow-moving Report (>30 days no sale)
- Auto stock update on confirmed delivery

### 🔸 Delivery Management
- Memo Number entry
- Partial delivery & return support
- Per-address delivery: ✅ Multiple times/day allowed
- Load Sheet by Route/Zone (PDF & Excel)
- Delivery confirmation updates reports, stock, and ledgers

### 🔸 Cash & Bank Book
- Shows opening cash/bank balances
- Description dropdown + manual entry
- Cheque number field
- Entry: All roles
- Balance view: Admin, Manager, Accountant only

### 🔸 Profit & Loss Report
- Basis: Cash
- Includes non-stock sales, commissions, and damaged product sales
- PDF/Excel/Google Sheets export
- Access: Admin, Manager, Accountant

### 🔸 Balance Sheet
- Basis: Accrual
- Advances from customers marked as liability

### 🔸 CRM (Customer/Supplier/Dealer)
- Auto-approval after 2 hours (optional)
- Manual approval allowed by Admin/Manager/Accountant
- Duplicate detection & rejection system
- File upload: NID, License, Agreements

### 🔸 Task & Reminder System
- Customer-specific tasks (Follow-ups, Deliveries, Cheques)
- Role-based reminders

### 🔸 Route/Zone-wise Sales Mapping
- Group customers by zone
- Compare sales performance by area
- Access: All roles

### 🔸 Non-Stock Product Sales
- For services or custom items
- Do not affect inventory
- Tagged and tracked in revenue

### 🔸 Price Change History
- Logs user, old/new price, timestamp
- Admin-only view, exportable

### 🔸 Internal User Logs
- Track actions like entry, update, delivery, stock transfer
- Access: Admin/Manager

### 🔸 Plugin/API Marketplace
- SMS/WhatsApp Gateway (Ajura/Twilio)
- Future integration-ready for payment gateways

### 🔸 Backup & Security
- Auto Google Drive backup
- Daily at fixed time

---

## 📱 Mobile App Features (MKR Enterprise)

- Native Android App
- Full offline data entry + auto sync every 1 min
- Background sync even when screen is off
- Sync Progress Indicator on top bar
- PDF invoice generation and WhatsApp sharing
- Dark/Light Mode, Bangla/English language toggle
- Role-based access control
- Modules: Login, Sales, Delivery, Purchase, CRM, Stock, Reports, Notifications

---

## 🛡️ Roles & Permissions

| Module                        | Admin | Manager | Sales | Delivery | Accountant |
|------------------------------|:-----:|:-------:|:-----:|:--------:|:----------:|
| Sales Entry                  | ✅    | ✅      | ✅    | ❌       | ❌         |
| View Invoice                 | ✅    | ✅      | ✅    | ✅       | ✅         |
| Edit After Delivery          | ✅    | ❌      | ❌    | ❌       | ❌         |
| Delivery Confirmation        | ✅    | ✅      | ❌    | ✅       | ❌         |
| Cash/Bank Book Entry         | ✅    | ✅      | ✅    | ❌       | ✅         |
| View Cash/Bank Balance       | ✅    | ✅      | ❌    | ❌       | ✅         |
| View P&L Report              | ✅    | ✅      | ❌    | ❌       | ✅         |
| View Balance Sheet           | ✅    | ✅      | ❌    | ❌       | ✅         |
| View Profit Per Invoice      | ✅    | ✅      | ✅    | ✅       | ✅         |
| Access Internal Logs         | ✅    | ✅      | ❌    | ❌       | ❌         |
| Add Customer/Supplier        | ✅    | ✅      | ✅    | ❌       | ✅         |

---

## 🗓️ Telegram Reporting Schedule

- Daily Report: 9:00 PM
- Weekly Summary: Every Thursday at 9:00 PM
- Monthly Summary: Every 30/31st at 9:00 PM
- Includes: Sales, Discounts, Deliveries, Cash Summary

---

## 🧾 Zone-wise Van Load Sheet (Daily)

- Route/Zone filter: e.g., Koyra, Bedkasi, Amadi
- Products grouped by customer and address
- Delivery quantity, contact, and pending status
- One PDF/Excel file per day
- Supports multiple products per customer

📄 [Download PDF Template](#)  
🧾 [Download Excel Template](#)  
📱 [Mobile View Mockup](#)

---

## 🧪 Developer Setup

```bash
git clone https://github.com/nazmussakib42/mkrenterprise-frontend.git
cd mkrenterprise-frontend
npm install
npm run dev
