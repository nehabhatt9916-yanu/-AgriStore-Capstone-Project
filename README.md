# -AgriStore-Capstone-Project
End-to-End Business Analysis Capstone Project for an Online Agriculture Products Store
# 🌾 AgriStore — Online Agriculture Products Store

> A CSR-driven digital platform connecting farmers directly with verified manufacturers of seeds, fertilizers, and pesticides. Built by APT IT Solutions for SOONY Company.

---

## 📌 Project Overview

| Field | Details |
|---|---|
| **Project Sponsor** | Mr. Henry / SOONY Company |
| **Client** | SOONY (CSR Initiative) |
| **Development Company** | APT IT Solutions |
| **Project Manager** | Mr. Vandanam |
| **Business Analyst** | Mrs. Neha Bhatt |
| **Budget** | INR 2 Crores |
| **Duration** | 18 Months |
| **SDLC Model** | V-Model |
| **Technology** | Java (3-Tier Architecture) |

AgriStore is a web and mobile application that enables farmers in remote areas to browse, compare, and purchase agricultural products directly from certified manufacturers — with doorstep delivery, real-time order tracking, and multiple digital payment options.

---

## 🎯 Problem Statement

Farmers like Peter, Kevin, and Ben in rural India face significant challenges:

- Physically traveling long distances to procure seeds, fertilizers, and pesticides
- Dependence on costly middlemen with no price transparency
- Cash-only transactions with no digital receipts
- Zero order tracking or reliable delivery timelines
- Limited access to product information and quality assurance

AgriStore eliminates these barriers through a purpose-built digital platform.

---

## ✨ Key Features

### For Farmers
- **Registration & Login** — Secure onboarding with Aadhaar, mobile, and email
- **Product Catalog** — Browse seeds, fertilizers, pesticides from verified manufacturers
- **Search & Filter** — Filter by category, brand, price range, and rating
- **Shopping Cart** — Add, update, and manage cart items before checkout
- **Multiple Payment Options** — UPI, Net Banking, Credit/Debit Cards, Cash on Delivery
- **Order Tracking** — Real-time status from placement to doorstep delivery
- **Reviews & Ratings** — Rate products and read peer farmer reviews
- **Order History** — View past orders with downloadable invoices

### For Manufacturers
- **Onboarding & Verification** — Admin-verified manufacturer accounts
- **Product Management** — Upload, edit, and manage product listings with images and certifications
- **Order Management** — View and update the status of received orders

### For Admins
- **Dashboard** — Manage users, manufacturers, products, orders, and payments
- **Product Approval** — Review and approve manufacturer listings before public display
- **Reporting** — Generate sales, user activity, and inventory reports

---

## 🏗️ Architecture

AgriStore uses a **3-Tier Architecture**:

```
┌─────────────────────────────────────────────────────┐
│             PRESENTATION TIER (UI)                  │
│        React.js / Angular, HTML5, CSS3, JS          │
└──────────────────────┬──────────────────────────────┘
                       │ HTTP/HTTPS
┌──────────────────────▼──────────────────────────────┐
│          APPLICATION TIER (Business Logic)          │
│       Java (Spring Boot), REST APIs, Tomcat         │
└──────────────────────┬──────────────────────────────┘
                       │ JDBC / Hibernate ORM
┌──────────────────────▼──────────────────────────────┐
│              DATA TIER (Database)                   │
│           MySQL / PostgreSQL, Hibernate             │
└─────────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | React.js / Angular, HTML5, CSS3, JavaScript |
| **Backend** | Java (Spring Boot), REST APIs |
| **Application Server** | Apache Tomcat |
| **Database** | MySQL / PostgreSQL |
| **ORM** | Hibernate, JDBC |
| **Cloud** | AWS / GCP |
| **Version Control** | Git |
| **Project Management** | JIRA |
| **Testing** | Selenium, JUnit |

---

## 📋 Requirements Summary

### Functional Requirements (Sample)

| ID | Requirement | Priority |
|---|---|---|
| FR0001 | Farmer Registration (name, mobile, email, Aadhaar) | 8/10 |
| FR0002 | Product Search by category, filter | 8/10 |
| FR0005 | Shopping Cart management | 9/10 |
| FR0006 | Order Placement with address | 9/10 |
| FR0007 | Payment Gateway (UPI/Card/COD) | 8/10 |
| FR0009 | Real-time Order Tracking | 8/10 |
| FR0012 | Manufacturer Registration & Verification | 9/10 |
| FR0013 | Manufacturer Product Upload | 9/10 |

### Non-Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| NFR0101 | Page load under 2 seconds on 3G | 9/10 |
| NFR0103 | 99.5% system uptime | 9/10 |
| NFR0104 | SSL/TLS encryption, 2FA | 10/10 |
| NFR0105 | Handle 10,000 concurrent users | 8/10 |
| NFR0106 | Fully responsive (mobile/tablet/desktop) | 9/10 |

---

## 🗓️ Project Timeline (V-Model)

```
Month:  1    2    3    4    5    6    7    8    9   10   11   12   13   14   15   16   17   18
        ├────┤
RG      ████
RA           ████████
Design            ████████
D1                        ████████████
T1                                    ████████
D2                                            ████████████
T2                                                        ████████
D3                                                                ████████████
T3                                                                            ████████
D4                                                                                    ████████
T4                                                                                            ████████
UAT                                                                                                    ██████████████
Deploy                                                                                                              ████████
```

**Total estimated effort: ~9,520 man-hours**

---

## 👥 Team

| Role | Person |
|---|---|
| Project Sponsor | Mr. Henry |
| Financial Head | Mr. Pandu |
| Project Coordinator | Mr. Dooku |
| Delivery Head | Mr. Karthik |
| Project Manager | Mr. Vandanam |
| Business Analyst | Mrs. Neha Bhatt |
| Sr. Java Developer | Ms. Juhi |
| Java Developers | Mr. Teyson, Ms. Lucie, Mr. Tucker, Mr. Bravo |
| DB Admin | Mr. John |
| Network Admin | Mr. Mike |
| QA / Testers | Mr. Jason, Ms. Alekya |
| Farmer Representatives | Peter, Kevin, Ben |

---

## 🗄️ Database Schema (Key Tables)

```
USERS ──────────────── FARMER_PROFILE
  │                    MANUFACTURER_PROFILE
  │
PRODUCTS ──────────── PRODUCT_IMAGES
  │
ORDERS ─────────────── ORDER_ITEMS
  │                    PAYMENTS
  │                    ORDER_TRACKING
  │
REVIEWS ────────────── (linked to PRODUCTS + FARMER_PROFILE)
```

---

## 🔐 Security

- SSL/TLS encryption for all data in transit
- Passwords stored as bcrypt hashes
- Two-Factor Authentication (2FA)
- Secure third-party payment gateway integration (Razorpay / PayU)
- Role-based access control (FARMER / MANUFACTURER / ADMIN)

---

## 📊 Business Objectives

1. Reduce farmer procurement time by **80%**
2. Eliminate middlemen to reduce costs by **20–30%**
3. Provide **24/7** access to quality agricultural products
4. Support **10,000+ farmers** within the first year
5. Enable direct manufacturer-to-farmer communication

---

## 💰 Billing Model

SOONY selected the **Time & Material (Billing) Model**:
- Fortnightly timesheet submission
- 3-day client verification cycle
- Quarterly audits

---

## 🚀 Success Criteria

- Application live within 18 months and INR 2 Crore budget
- Minimum **1,000 registered farmers** in Month 1
- System uptime of **99.5%**
- Page load time under **2 seconds**

---

## 📄 Documentation Produced

- Business Requirements Document (BRD)
- Functional Requirements Specification (FRS)
- Use Case Diagram & Specifications
- Activity Diagrams & Data Flow Diagrams (DFD)
- ER Diagram & Database Schema
- Wireframes & Prototypes (5 screens)
- Requirements Traceability Matrix (RTM)
- Risk Register
- RACI Matrix
- Gantt Chart
- UAT Plan & Test Cases
- Project Closure Document

---

## 👩‍💼 Role & Responsibilities

### Business Analyst – Neha Bhatt

- Requirement Gathering
- Stakeholder Communication
- Documentation Preparation
- Wireframing & Prototyping
- Use Case Modeling
- Risk & Gap Analysis
- UAT Coordination
- Change Management
- RTM Maintenance

---

## 📚 Learning Outcomes

Through this project, I gained hands-on experience in:

- Business Analysis
- SDLC Methodologies
- Requirement Engineering
- UML Modeling
- Stakeholder Management
- Agile & V-Model Concepts
- Testing & UAT
- Documentation Standards

---

## 🚀 Future Enhancements

- Multi-language support
- Farmer crop auction system
- AI-based crop recommendations
- Government scheme integration
- Mobile application launch

---

## 📎 Repository Structure

```bash
AgriStore-Capstone-Project/
│
├── BRD & Business Documents
├── UML Diagrams
├── Wireframes
├── RTM & Test Cases
├── Project Planning Documents
├── Screenshots
└── README.md
🤝 Connect With Me

👩‍💼 Neha Bhatt
💼 Business Analyst Aspirant
🌱 Passionate about Digital Transformation & AgriTech

⭐ If You Like This Project

Feel free to:

Star this repository
Share feedback
Connect with me on LinkedIn
www.linkedin.com/in/neha-bhatt-aa49b33a5

---

*"Grow good. Live good." — AgriStore*

