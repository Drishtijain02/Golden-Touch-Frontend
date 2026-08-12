# ✨ Golden Touch Beauty Salon

A modern, responsive **full-stack salon website and appointment management system** built for **Golden Touch Beauty Salon & Parlour**.

The project is designed to provide customers with a premium online experience while giving the salon owner a secure dashboard to manage appointments, services and offers.

🔗 **Live Website:** https://golden-touch-frontend.vercel.app/

---

## 🌸 About the Project

Golden Touch is a real-world salon website developed to bring the salon's services, portfolio, offers and appointment booking into one professional digital platform.

Unlike a simple static salon website, the project includes a **customer-facing website + backend API + database + owner dashboard**, allowing the salon to manage its day-to-day bookings digitally.

The website is currently deployed and being used as a real business project.

---

## 🚀 Key Features

### 👩‍💼 Customer Website

* ✨ Premium and responsive salon website
* 📱 Mobile-friendly design
* 🏠 Home, About, Services, Gallery and Contact sections
* 👩‍🎨 Founder/Owner profile section
* 💇 Detailed service catalogue
* 🖼️ Salon and service gallery
* 🏷️ Offers and promotional sections
* 📍 Salon location and contact information
* 📅 Online appointment booking
* 📋 Customer appointment form
* 📧 Customer email collection for booking communication

### 📅 Appointment Management

Customers can submit an appointment request directly through the website.

Each appointment stores information such as:

* Customer name
* Phone number
* Email
* Selected service
* Preferred date
* Preferred time
* Special requests
* Booking ID
* Appointment status
* Booking creation time

Appointments follow a simple workflow:

**Pending → Confirmed → Completed**

Appointments can also be cancelled or deleted from the owner dashboard.

### 🖥️ Owner Dashboard

The salon owner has access to a dedicated password-protected dashboard.

The dashboard allows the owner/manager to:

* 🔐 Securely log in
* 📊 View appointment statistics
* 📅 View all appointments
* 🔎 Filter appointments by status/date
* 👤 View complete customer details
* ✅ Confirm appointments
* ✔️ Mark appointments as completed
* ❌ Cancel/delete appointments
* 💬 Send confirmation messages through WhatsApp
* 📱 Contact customers directly
* 🏷️ Manage website content such as services and offers

### 🔄 Dynamic Website Management

One of the main goals of the project is to reduce the salon's dependency on a developer for everyday updates.

The owner/manager can manage website content through the dashboard.

For example:

**Owner adds a new service → Service appears on the website**

**Owner adds a new offer → Offer appears on the website**

This makes the website easier to maintain as the business grows.

### 📧 Email Integration

The system integrates email notifications for appointment bookings.

When a customer submits an appointment:

**Customer → Website → Backend → Database → Owner Email**

The owner receives the booking information by email and can then open the owner dashboard to manage the appointment.

---

## 🏗️ Project Architecture

```text
Customer
   │
   ▼
Golden Touch Website
   │
   │ Appointment Request
   ▼
Backend API
   │
   ├──────────────► Supabase Database
   │
   └──────────────► Resend Email Service
                         │
                         ▼
                    Owner Email
                         │
                         ▼
                  Owner Dashboard
                         │
                         ▼
              Appointment Management
```

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* Responsive Design
* Font Awesome
* Google Fonts

### Backend

* Node.js
* Express.js
* REST API
* JavaScript

### Database & Authentication

* Supabase
* Supabase Authentication
* PostgreSQL database

### Email

* Resend

### Deployment

* Vercel

---

## 📂 Project Structure

```text
golden-touch/
│
├── frontend/
│   ├── index.html
│   ├── dashboard.html
│   ├── ...
│
├── backend/
│   ├── routes/
│   │   ├── appointments.js
│   │   ├── auth.js
│   │   └── ...
│   │
│   ├── services/
│   │   └── emailService.js
│   │
│   ├── config/
│   │   ├── supabase.js
│   │   └── supabaseAuth.js
│   │
│   ├── middleware/
│   │   └── validation.js
│   │
│   └── server.js
│
└── README.md
```

---

## 🔐 Security

The project uses a separate owner dashboard with authentication so that appointment and business-management functionality is not publicly accessible.

Sensitive credentials such as API keys and database keys are stored using environment variables rather than being exposed in the frontend code.

```text
RESEND_API_KEY=your_key
OWNER_EMAIL=owner@example.com
SUPABASE_URL=your_url
SUPABASE_SERVICE_ROLE_KEY=your_key
```

> Never commit `.env` files or private API keys to GitHub.

---

## 📧 Appointment Flow

```text
1. Customer opens website
          ↓
2. Customer selects service
          ↓
3. Customer fills appointment form
          ↓
4. Backend validates request
          ↓
5. Appointment stored in Supabase
          ↓
6. Owner receives email notification
          ↓
7. Owner opens dashboard
          ↓
8. Owner confirms appointment
          ↓
9. WhatsApp confirmation can be sent
          ↓
10. Appointment status becomes Confirmed
```

---

## 📊 Dashboard Workflow

| Status       | Meaning                               |
| ------------ | ------------------------------------- |
| 🟡 Pending   | New appointment awaiting confirmation |
| 🟢 Confirmed | Appointment accepted by salon         |
| 🔵 Completed | Customer's appointment completed      |
| 🔴 Cancelled | Appointment cancelled                 |

---

## 📱 Responsive Design

The website is designed to work across:

* 💻 Desktop
* 💻 Laptop
* 📱 Mobile
* 📲 Tablet

The interface adapts to different screen sizes while maintaining the salon's premium visual identity.

---

## 🎯 Project Goals

The main goals of the project were to:

* Build a professional online presence for a real salon
* Make appointment booking easier for customers
* Digitize appointment management
* Reduce manual booking communication
* Give the salon owner control over website content
* Provide automatic booking notifications
* Create a scalable foundation for future features

---

## 🔮 Future Improvements

Potential future improvements include:

* 💳 Online payment integration
* 📅 Calendar-based appointment availability
* ⏰ Automated appointment reminders
* 🎁 Automated promotional emails
* 👥 Customer accounts
* 📈 Advanced business analytics
* 📊 Revenue and booking reports
* ⭐ Customer review management
* 📱 Progressive Web App support

---

## 👩‍💻 Developed By

**Drishti Jain**

Designed and developed as a real-world full-stack web development project for Golden Touch Beauty Salon & Parlour.

---

## 📄 License

This project was developed specifically for Golden Touch Beauty Salon & Parlour.

© 2026 Golden Touch Beauty Salon & Parlour
