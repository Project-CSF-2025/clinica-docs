# Clinic Incident Reporting System – Full Project Overview

This is a full-stack web application designed to allow hospital or clinic staff to submit anonymous incident reports. The system improves communication and safety by enabling secure, trackable interactions between staff and administrators.

This project is divided into two separate repositories:

- 🔗 [Frontend Repository](https://github.com/Project-CSF-2025/clinica-front-public)  
- 🔗 [Backend Repository](https://github.com/Project-CSF-2025/clinica-back-public)

---

## Project Summary

The application enables clinical staff to report incidents through an anonymous form, and allows administrators to manage those reports in a private dashboard. Each report is tracked with a unique code, allowing both communication and follow-up without revealing user identity.

---

## Tech Stack

### Frontend:
- React (with Vite)
- JavaScript (ES6+)
- Bootstrap & MUI
- Environment config via `.env`

### Backend:
- Node.js with Express
- SQL Server
- JWT authentication
- Multer for file uploads
- Nodemailer for emails

---

## 🔧 How It Works

- **Users** can:
  - Fill and submit an anonymous report form
  - Attach optional files (images or PDFs)
  - Optionally provide an email for notifications

- **Admins** can:
  - Log in securely using JWT-based auth
  - View reports, update status, and add internal notes
  - Exchange messages with anonymous users
  - Download data and attachments

---

## Communication Between Frontend and Backend

- The frontend uses a `.env` variable (`VITE_API_URL`) to define the API base URL.
- The backend exposes routes for reports, messaging, login, status tracking, and file handling.
- CORS is enabled to allow frontend/backend communication.

---

## Repositories Breakdown

### 🔸 Backend Repository

**URL:** [clinica-back-public](https://github.com/Project-CSF-2025/clinica-back-public)

Includes:

- Admin login system with JWT
- File upload logic with Multer
- Email notifications with Nodemailer
- SQL Server database schema
- Anonymous incident handling logic
- Fully documented `.env` setup and database usage

### 🔸 Frontend Repository

**URL:** [clinica-front-public](https://github.com/Project-CSF-2025/clinica-front-public)

Includes:

- Anonymous reporting form
- Admin dashboard at `/admin`
- Messaging interface for follow-ups
- Report review and filtering UI
- JSON-powered dropdowns (departments, professions, etc.)

---

## Authors

- **Pragati Juyal** – Backend developer & full-stack coordination  
- **Kanako Inamine** – Frontend development & UI/UX

---

## License

This project is licensed under the [MIT License](./LICENSE).  
It is provided as-is and the authors are not liable for any damages.  
Use in production is permitted with proper credit.


