# 🏢 MKR Enterprise

**A B2B & B2C ERP system** tailored for inventory, delivery, sales, accounts, and performance management for small and medium businesses.

---

## 📦 Core Features

### 🔹 Sales Module
- Walk-in Showroom Sales: No customer entry required
- Invoice profit auto-calculated (non-editable)
- All users can view invoices and profits
- Editable **only before delivery** (Admin only)

### 🔹 Purchase & Inventory
- FIFO method used for inventory cost valuation
- Product return and stock reconciliation supported
- Supports non-stock product sales (services, custom items)

### 🔹 Delivery Management
- Zone-wise Van Load Sheet generation (A4 format)
- One customer may receive **multiple products**
- Multiple deliveries per address per day
- Delivery confirmation required to update stock & reports
- Return management, pending-delivery tracking

### 🔹 Cash Book & Bank Book
- Opening Cash in Hand and Bank auto shown
- Manual entry by any user
- Balance visibility only for: Admin, Manager, Accountant
- Cheque number + description field (with dropdown/manual input)

### 🔹 Customer & Supplier Management
- Add/Edit/Delete with duplicate check
- Upload documents (NID, Trade License, Agreement)
- Optional auto-approval after 2 hours
- Manual approval allowed for: Admin, Accountant, Manager

---

## 📊 Reporting & Finance

### 🔸 Profit Per Invoice Report
- Auto-calculated profit (cannot be edited)
- Accessible by all users
- Includes margin alerts & profit % threshold config

### 🔸 Route/Zone-wise Sales Mapping
- Group performance by delivery zone (e.g., Koyra, Gilabari, Amadi)
- Compare sales data across zones
- Works with Load Sheet Generator

### 🔸 Statement of Profit or Loss
- Cash Basis by default
- Includes Other Income: (e.g., damaged product sales, commissions)
- Export to PDF, Excel, Google Sheets

### 🔸 Balance Sheet
- Accrual Basis by default
- Toggle between Cash vs Accrual (default: P&L = Cash, BS = Accrual)

### 🔸 Dead Stock & Slow Moving Report
- Alerts for products unsold for 30+ days

### 🔸 Aging Report (Receivables & Payables)
- Buckets: 0–30, 31–60, 61–90, >90 days
- Exportable, filterable

---

## 📱 Mobile App (Private APK)

- Full offline data entry (auto sync every 1 minute)
- Background sync while screen off
- Role-based access
- PDF invoice/receipt with WhatsApp share
- Modules: Sales, Delivery, Expense, Stock, Tasks, Documents, etc.
- Languages: English, Bangla
- Dark/Light Mode

---

## 🔐 Roles & Permissions

| Feature                        | Admin | Manager | Accountant | Sales | Delivery |
|-------------------------------|:-----:|:-------:|:----------:|:-----:|:--------:|
| View Profit per Invoice       | ✅    | ✅      | ✅         | ✅    | ✅       |
| Edit Invoices after Delivery  | ✅    | ❌      | ❌         | ❌    | ❌       |
| Cash/Bank Balance View        | ✅    | ✅      | ✅         | ❌    | ❌       |
| Delivery Confirmation         | ✅    | ✅      | ❌         | ❌    | ✅       |
| Input Discount                | ✅    | ✅      | ✅         | ✅    | ✅       |

---

## 🧾 Automation & Alerts

- **Telegram Reports:**
  - Daily Summary @ 9 PM
  - Weekly Summary (Thursday 9 PM)
  - Monthly Summary (30th/31st @ 9 PM)
  - Discount Summary Included

- **WhatsApp & SMS:**
  - Delivery confirmations
  - Stock alerts
  - Payment reminders

- **Sync Alerts:**
  - Top bar indicator: “All Data Synced”
  - Failsafe: Retry on failure

---

## 🧰 Utilities & Advanced

- **Document Uploads** per customer
- **Task & Reminder System**
- **Internal User Activity Log**
- **Plugin/API Marketplace Ready**
- **Auto Backup to Google Drive (Daily)**

---

## 📤 Export Formats

- PDF (Invoices, Load Sheets, Reports)
- Excel/CSV (Reports, Ledgers)
- Google Sheets (Profit & Loss, Stock Reports)

---

## 📂 File Download Templates

- ✅ [Zone-wise Load Sheet – PDF](./ZoneWise_LoadSheet_Koyra_Grouped.pdf)
- ✅ [Zone-wise Load Sheet – Excel](./ZoneWise_LoadSheet_Koyra_Grouped.xlsx)

---

## 🧑‍💻 Tech Stack

- **Frontend**: React + Vite + Tailwind CSS
- **Backend**: Supabase (PostgreSQL + Auth)
- **App**: Flutter (Offline-first support)
- **Deployment**: Vercel (Frontend), GitHub (Version Control)

---

## 📌 Project Setup

```bash
git clone https://github.com/nazmussakib42/mkrenterprise-frontend.git
cd mkrenterprise-frontend
npm install
npm run dev
