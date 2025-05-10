# 🏗️ Construction Management Web Portal

## 📌 Overview
This Construction Web Portal is a full-featured ERP-style application tailored to construction businesses. It integrates core operational tools with advanced features like FreshBooks syncing, digital signatures, SMS alerts, and third-party integrations.

---

## 🧱 Core Modules

### 1. Authentication & Access Control
- Discord/Email/SSO login (optional)
- Role-Based Access Control (RBAC)
- Admin, HR, Manager, Foreman, Employee, Client roles

### 2. Project Management
- Create/manage construction projects
- Task lists, Gantt charts, daily logs, delays
- Budget tracking and milestone control
- Assign teams and employees

### 3. FreshBooks Integration
- Sync proposals, estimates, and invoices
- View FreshBooks documents in-app
- Track client payments and statuses
- Link FreshBooks clients to internal records
- Webhook-based updates

### 4. Job Estimation & Bidding
- Client-side approval workflows
- Auto-generate projects from approved estimates
- Attach e-signatures to proposals
- Include scope of work, labor, material breakdowns

### 5. Time Tracking & Scheduling
- GPS-based clock-in/out
- Shift and crew assignment calendar
- Timesheet logs and exports
- Site-wise attendance and time approval

### 6. Document & Blueprint Management
- Upload blueprints, permits, drawings
- Tag-based search and version control
- Role-based access to documents

### 7. Inventory & Material Management
- Track per-site material use
- PO creation and low-stock alerts
- Tool/equipment logs and assignments
- Auto-calculate job material consumption

### 8. Fleet Management
- Assign vehicles to projects/employees
- Maintenance reminders
- Track usage and license expirations
- Integration with GPS tracking (optional)

### 9. Field Service Reporting
- Mobile-friendly work reports
- Photos, notes, checklists
- Safety/incident forms
- Real-time syncing with project dashboards

### 10. Customer Portal
- View project status, invoices, documents
- Submit service requests or messages
- Access proposals and sign estimates

---

## 🧑‍💼 HR Suite

### 11. Employee Directory
- Profiles with roles, certifications, contact info
- Team assignments

### 12. Recruitment & Onboarding
- Job postings and application tracking
- Interview scheduling and offer flow
- New hire onboarding checklists

### 13. Leave & Attendance
- PTO/sick/vacation requests
- Approval workflows
- Team-based calendar view
- Time-off balance tracking

### 14. Payroll Integration
- Hourly/salary sync with timesheets
- Export-ready for Gusto, QuickBooks, ADP
- Auto-calculate overtime

### 15. Certification & Compliance
- OSHA, safety, license tracking
- Alerts for expiring qualifications
- Required certifications by job type

### 16. Performance Tracking
- Project-based evaluations
- KPI tracking: punctuality, quality, incidents
- Disciplinary log

### 17. Equipment Assignment
- Issue & return logs for tools/PPE
- Damage/replacement tracking
- Uniform assignment tracking

---

## 🔧 System Features

### ✍️ E-Signature Support
- Signature pad or typed option
- Auto-insert into PDFs
- Signature logs and audit trail

### 📲 SMS Notifications
- Job updates, appointment reminders
- Admin alerts and deadline warnings
- Two-way SMS (via Twilio or similar)

### 🔌 API & Integrations
- REST API with token-based access
- Webhooks for internal event tracking
- Google Workspace Integration:
  - Sync tasks/events to Google Calendar
  - Attach Google Drive documents to projects
  - Import onboarding forms/sheets

### 📤 Exports & Reporting
- Export project reports, timesheets, invoices
- PDF, Excel, and CSV formats
- Download job cards and safety documentation

---

## 📊 Dashboards & Analytics
- Project progress dashboard
- HR metrics: headcount, leave, certification
- Financial dashboard: unpaid invoices, project costs
- Material usage, fleet status, task completion

---

## 🚀 Tech Stack (Recommended)
- **Frontend:** Next.js + React + Tailwind CSS + shadcn/ui
- **Backend:** Node.js + Express or Fastify
- **Database:** MongoDB Atlas or PostgreSQL
- **Auth:** JWT or Discord OAuth2
- **Hosting:** Vercel (Frontend) + Railway (Backend)
- **Third-Party Services:** FreshBooks API, Twilio SMS, Google Workspace API

---

## 📂 Suggested File Structure
```
/src
  /app
    /projects
    /clients
    /invoices
    /field-service
    /hr
    /fleet
    /inventory
    /auth
    /api
/components
/lib
/utils
```

---

## ✅ Next Steps
- [ ] Set up Next.js frontend scaffold
- [ ] Define user roles and auth flow
- [ ] Set up MongoDB collections and Mongoose schemas
- [ ] Build API routes for core modules
- [ ] Integrate FreshBooks via API keys
- [ ] Add E-Signature and SMS providers
- [ ] Document REST API for third-party access
