# 🛠️ Handyman Company Web Portal – Feature Specification

_Last Updated: May 06, 2025_

---

## 🔧 1. Job Management Module

### Features
- Create and manage **Job Proposals**, **Estimates**, and **Invoices**
- Push proposals/estimates/invoices to **FreshBooks**
- Attach **Terms & Conditions / Contracts** to:
  - Proposals (for large jobs)
  - Estimates (for small jobs)
- Include **Customer & Site Information** fields

### Integration
- FreshBooks API for syncing financial documents

---

## 👤 2. Customer Management Module

### Features
- Track customer records, job history, and contact info
- Assign estimates and invoices to customers
- Customer portal access (secure login)
  - View proposals, approve estimates, view/pay invoices

### Integration
- Sync customer records with **FreshBooks**
- Store and use `freshbooks_client_id` for mapping

---

## 🚚 3. Fleet Management Module

### Features
- Assign vehicles to employees
- View live GPS data (via external GPS provider)
- Track mileage logs per job/employee
- Schedule vehicle maintenance

---

## ⏱ 4. Employee Time Tracking Module

### Features
- Clock In / Clock Out functionality (mobile-friendly)
- Geo-location tracking on clock events
- Weekly/hourly summaries and discrepancy reports

---

## 📦 5. Inventory Management Module

### Features
- Track tools, materials, and job-site inventory
- Assign items to jobs or employees
- Low stock alerts and reorder tracking

---

## 🛠 6. Technician Reporting & Ticketing Module

### Features
- Create service tickets with job/site/customer info
- Assign tickets to technicians
- Status tracking: Scheduled → In Progress → Complete
- Technician can add job notes, photos, and materials used

---

## 🧑‍🔧 7. Employee Management Module

### Features
- Employee profile management:
  - Name, role, status, contact info
  - Assigned vehicle & tool tracking
- Show real-time GPS of assigned vehicle
- Time tracking integration: show hours worked
- View all assigned equipment/tools

### Document Management
- Upload employee-related documents (e.g. ID, certs, contracts)
- View-only for employees (optional)
- Admin/HR full access to upload/download/delete

---

## 📋 8. Human Resources (HR) Module

### Features
- Create and manage **write-ups** and **corrective actions**
- Track incident details, linked job/ticket, and required actions
- Upload and attach supporting documentation
- Auto-link write-up acknowledgments to employee documents
- Secure view of employee HR history

### Permissions
- HR/Admin only access to view/edit HR records
- Employees can view their own signed documents (optional)

---

## 🔐 System & Integration Notes

- Authentication with Role-Based Access Control (Admin, HR, Technician, Customer)
- API integrations:
  - **FreshBooks** for estimates/invoices/clients
  - **GPS/Geo API** for fleet and time tracking
  - **Cloud storage** (e.g., AWS S3) for document uploads

---

## 📁 Future Enhancements

- Payroll exports from Time Tracking
- QuickBooks integration alternative
- Push notifications for assigned jobs or HR actions
- Internal messaging/alerts system

