# 🌐 MKR Enterprise - Full ERP System (B2B & B2C)

**MKR Enterprise** is a complete Business ERP & Delivery Management system designed for wholesale and retail businesses. It includes inventory, cash flow, profit tracking, customer management, delivery coordination, and reporting — all optimized for both desktop and mobile.

---

## 🧭 Project Type

- **ERP System**: B2B & B2C
- **Tech Stack**: React (Vite), Tailwind CSS, Supabase, Telegram/WhatsApp APIs
- **App**: Native Android (Offline-first)

---

## 📦 Core Modules

| Module                         | Description                                                                 |
|-------------------------------|-----------------------------------------------------------------------------|
| ✅ Sales (Showroom/Dealer)     | Support for walk-in and registered customers, instant invoice generation   |
| ✅ Purchase                    | With supplier dropdown, auto stock adjustment, ledger update               |
| ✅ Inventory Management        | FIFO method, stock ledger, alerts, and dead stock report                   |
| ✅ Delivery Management         | Van-wise Load Sheet, memo input, return handling, partial delivery allowed |
| ✅ Profit per Invoice          | Auto-calculated, viewable by all, editable only by Admin after delivery    |
| ✅ Non-Stock Product Sales     | Service/custom sales tracked separately without affecting inventory        |
| ✅ Customer Management         | Document upload (NID, License), task/reminder linked                       |
| ✅ Supplier Management         | Same structure as customer                                                 |
| ✅ Expense Tracker             | Cash/bank-based expense input                                              |
| ✅ Task & Reminder System      | Per customer task tracking, due-dates, notifications                       |
| ✅ Cash Book & Bank Book       | Daily in/out, opening balance, visible only to Accountant/Admin/Manager    |
| ✅ Statement of Profit/Loss    | With other income, monthly summary to email                                |
| ✅ Balance Sheet (Accrual)     | Toggle option: Cash basis or Accrual basis                                |
| ✅ Internal Activity Log       | Logs every major user activity for admin audit                             |
| ✅ WhatsApp/Telegram Alerts    | SMS/WhatsApp for delivery, due, and summary reports                        |
| ✅ Document Uploads            | Linked per customer for licenses, agreements                              |
| ✅ Route/Zone-wise Sales Map   | Assign routes, track delivery/sales performance per zone                   |
| ✅ Load Sheet Generator        | Print A4 size sheet by Van/Zone, product grouped per customer              |
| ✅ Digital Signature (Admin)   | Used in invoices, challans                                                 |
| ✅ Dealer/Sub-dealer Panel     | Price margin, document upload, task link                                  |
| ✅ Mobile App                  | Offline data entry, background sync, full role features                    |
| ✅ Auto Approval (Customer)    | New customers auto-approved after 2 hours                                  |
| ✅ Aging Report                | Receivables/Payables by aging bucket                                       |
| ✅ Price Change History        | Logs user, time, old vs new price                                          |
| ✅ E-Commerce Catalog          | Public product listing with limited data                                   |
| ✅ Backup to Google Drive      | Auto-export daily                                                          |
| ✅ API/Plugin Marketplace      | Future support for payment/SMS integrations                               |

---

## 🧑‍💼 User Role Matrix

| Feature/Module           | Admin | Manager | Accountant | Sales | Delivery |
|--------------------------|:-----:|:-------:|:----------:|:-----:|:--------:|
| View Sales/Invoice       | ✅    | ✅      | ✅         | ✅    | ✅       |
| Edit After Delivery      | ✅    | ❌      | ❌         | ❌    | ❌       |
| View Profit per Invoice  | ✅    | ✅      | ✅         | ✅    | ✅       |
| Add/Edit Cash Book       | ✅    | ✅      | ✅         | ✅    | ❌       |
| View Balance             | ✅    | ✅      | ✅         | ❌    | ❌       |
| Approve Customer/Supplier| ✅    | ✅      | ✅         | ❌    | ❌       |
| Confirm Delivery         | ✅    | ✅      | ❌         | ❌    | ✅       |
| Access P&L Report        | ✅    | ✅      | ✅         | ❌    | ❌       |

---

## 🚚 Zone-wise Load Sheet

- One printable sheet per Van per day
- Grouped by:
  - Route/Zone
  - Customer
  - Multiple Products per Customer
- Contains:
  - Product Name
  - Quantity
  - Delivery Address
  - Contact
  - Memo Number
- Delivery person signs after confirmation
- Auto-logs returned/pending quantities
- A4 Printable Format

📄 [Download Load Sheet (PDF)](link-here)  
🧾 [Download Load Sheet (Excel)](link-here)  
📱 Mobile Preview: [Figma/mockup here]

---

## 📲 Mobile App Features

- Native Android (iOS later)
- Works Offline, Syncs every 1 minute
- Background Sync (while screen off)
- Sync Progress Indicator
- Multi-language: Bangla 🇧🇩 and English 🇬🇧
- Instant PDF Invoice, WhatsApp share
- Push Notifications for:
  - Order Updates
  - Payment Reminders
  - Delivery Confirmations

---

## 📆 Telegram Reporting Schedule

| Report Type         | Time         | Frequency   |
|---------------------|--------------|-------------|
| Discount Summary    | 9:00 PM      | Daily       |
| Weekly Summary      | 9:00 PM      | Every Thursday |
| Monthly Summary     | 9:00 PM      | 30/31st Day of Month |

---

## ⚙️ System Configs

- Minimum Profit Margin: **10%**
- One address can receive **multiple deliveries per day**
- FIFO Inventory Method
- P&L = **Cash Basis**, BS = **Accrual Basis**
- Sales: Walk-in customer doesn't require entry
- Data can be input even before approval
- Sync Interval: **1 minute**

---

## 🔧 Local Setup Instructions

```bash
git clone https://github.com/nazmussakib42/mkrenterprise-frontend.git
cd mkrenterprise-frontend
npm install
npm run dev
