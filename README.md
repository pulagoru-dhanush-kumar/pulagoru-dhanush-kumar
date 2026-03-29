<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=220&section=header&text=Dhanush%20Kumar%20Pulagoru&fontSize=42&fontColor=fff&fontAlignY=38&desc=Java%20Backend%20Developer%20%7C%20Spring%20Boot%20•%20JWT%20•%20AWS%20•%20MySQL&descSize=16&descColor=c9d1d9&descAlignY=58" />

<p>
  <img src="https://komarev.com/ghpvc/?username=pulagoru-dhanush-kumar&label=Profile+Views&color=0e75b6&style=flat-square" />
  <img src="https://img.shields.io/badge/Open%20To%20Work-Java%20Backend%20Developer-success?style=flat-square&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/📍-Hyderabad%2C%20India-orange?style=flat-square" />
</p>

</div>

---

## 👨‍💻 About Me

```java
@Component
public class DhanushKumar implements BackendDeveloper {

    private final String name        = "Dhanush Kumar Pulagoru";
    private final String role        = "Java Backend Developer (Transitioning from QA)";
    private final String current     = "Quality Analyst @ Santa Browser";
    private final String education   = "B.Tech CSE — VIT Bhimavaram | CGPA: 8.19";
    private final String email       = "dhanushvip1729@gmail.com";
    private final String portfolio   = "https://pulagoru-dhanush-kumar.github.io/Protfolio/";

    private final String[] strengths = {
        "Building production REST APIs with Spring Boot 3",
        "JWT Security, CORS, HMAC-SHA256 Payment Verification",
        "AWS EC2 + RDS deployment across 3 environments",
        "QA mindset → Rock-solid API validation & SQL data integrity"
    };

   
}
```

---

## 🚀 Featured Project — Messiah Vijaya Dairy E-Commerce Platform

<div align="center">

[![Live Demo](https://img.shields.io/badge/🌐%20Live%20Demo-Visit%20Now-blue?style=for-the-badge)](https://tinyurl.com/messiah-vijaya-dairy-pulagoru)
[![GitHub](https://img.shields.io/badge/📁%20Source%20Code-GitHub-black?style=for-the-badge&logo=github)](https://github.com/pulagoru-dhanush-kumar/vijaya-dairy)
[![Portfolio](https://img.shields.io/badge/🗂️%20Portfolio-View-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://pulagoru-dhanush-kumar.github.io/Protfolio/)

</div>

> **Production-ready full-stack dairy e-commerce platform** — Spring Boot REST APIs, deployed on AWS with 3 separate environments (Local → Staging → Production), Razorpay payment gateway, and JWT authentication.

### 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────────────────────┐
│                     VIJAYA DAIRY — SYSTEM OVERVIEW                  │
├──────────────────┬──────────────────────┬───────────────────────────┤
│    FRONTEND      │       BACKEND         │       DATABASE           │
│  HTML5 / CSS3    │  Spring Boot 3.2.5   │   AWS RDS MySQL 8.4       │
│  Vanilla JS      │  Spring Security     │   HikariCP Pooling        │
│  Responsive UI   │  JWT Authentication  │   Flyway Migrations       │
│  Razorpay SDK    │  Spring Data JPA     │   Automated Backups       │
└──────────────────┴──────────────────────┴───────────────────────────┘
                            │
              ┌─────────────┴─────────────┐
              │       AWS EC2             │
              │   Ubuntu 24.04 LTS        │
              │   t2.micro Instance       │
              └───────────────────────────┘
```

### 📡 REST API Summary (8 Controllers)

| Controller | Base Path | Methods | Highlights |
|---|---|---|---|
| 👤 User | `/users` | POST, GET | Login, Register, OTP, Forgot/Reset Password, JWT |
| 📦 Product | `/products` | POST, GET | Save, All, By Category |
| 🛒 Cart | `/cart` | POST, GET | Add, Increase, Decrease, Remove, View Cart |
| 💳 Payment | `/payment` | GET, POST | Checkout (Razorpay), Verify (HMAC-SHA256) |
| 📋 Order | `/orders` | GET, POST | My Orders, Modify Status |
| 📍 Address | `/api/address` | POST, GET | Save/Get logged-in user address |
| 🛡️ Admin | `/admin` | GET, POST, PUT, PATCH, DELETE | Full Product CRUD + Order Management |
| 🧪 Payment Test | `/test` | POST | Test Razorpay Signature Generation |

### 🗄️ Database Schema (8 Tables)

```
user ──────────── address        (1:1  via user_id FK)
user ──────────── cart           (1:1  via user_id FK)
cart ──────────── cart_item      (1:N  via cart_id FK)
product ────────── cart_item     (N:M  via product_id FK)
user ──────────── orders         (1:N  via user_id FK)
orders ─────────── order_products (N:M via order_id FK)
product ────────── order_products (N:M via product_id FK)
categories (lookup)
```

### ✅ Feature Breakdown

| Module | What's Built |
|---|---|
| 🔐 **Auth** | Register → OTP Email Verify → Login → JWT Token → Forgot/Reset Password |
| 🛒 **Cart** | Add item, Increase/Decrease quantity, Remove product, View cart with totals |
| 💳 **Payments** | Razorpay order creation → HMAC-SHA256 signature verification → Order update |
| 📦 **Products** | CRUD via Admin, Public listing by category, Base64 image support |
| 📋 **Orders** | User order history, Admin view all orders, Filter by status |
| 📍 **Address** | Save/update delivery address per user (JWT-scoped) |
| 🛡️ **Admin Panel** | Full product management, order analytics, status patching |
| 📧 **Email** | OTP delivery + Order confirmations via Gmail SMTP |

### 🌐 Deployment Environments

| Env | Server | Port | Branch | Database |
|---|---|---|---|---|
| 📱 Local | localhost | 8080 | develop | vijayadairy_local |
| 🧪 Staging | AWS EC2 — 3.107.228.182 | 8081 | staging | vijayadairy_staging |
| 🚀 Production | AWS EC2 — 32.236.15.39 | 8080 | main | vijayadairy (RDS) |

### 📊 Project Metrics

<div align="center">

| 💻 Code | 🗄️ DB | 🔌 APIs | 🌿 Branches | ⏱️ Hours | ✅ Commits |
|:---:|:---:|:---:|:---:|:---:|:---:|
| **2,000+ lines** | **8 tables** | **25+ endpoints** | **3** | **100+** | **20+** |

</div>

---

## 🛠️ Tech Stack

<div align="center">

**Core**

![Java](https://img.shields.io/badge/Java%2017-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot%203.2-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)

**Database & Cloud**

![MySQL](https://img.shields.io/badge/MySQL%208.4-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![AWS EC2](https://img.shields.io/badge/AWS%20EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)
![AWS RDS](https://img.shields.io/badge/AWS%20RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white)


**Tools & Testing**

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux%20%28Ubuntu%29-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Razorpay](https://img.shields.io/badge/Razorpay-02042B?style=for-the-badge&logo=razorpay&logoColor=white)

</div>

---

## 💼 Professional Experience

### 🏢 Quality Analyst — Santa Browser *(Feb 2025 – Present)*

> *Santa Browser is a cashback-enabled browser product with a complex rewards and transaction engine.*

- 🔌 **API Testing:** Tested cashback eligibility, wallet flows, refunds, and cancellation scenarios using **Postman** across multiple provider integrations *(Admitad, Cuelinks, CJ, Rakuten, Impact, Partnerize)*
- 🗄️ **SQL Validation:** Wrote SQL queries to validate user transactions, cashback status, and backend data integrity directly on production/staging databases
- 🐛 **Defect Tracking:** Managed test cases, defect lifecycles, and release coordination in **JIRA**
- 📊 **Analytics Validation:** Verified telemetry event firing, payload accuracy, and data consistency using **Requestly** and **Charles Proxy**
- 🤖 **Automation:** Built basic UI automation for regression flows using **Playwright**
- 🔔 **Push Notifications:** Tested push notification delivery across Android and Desktop platforms

> **Why this matters for backend dev:** Every API I built in Vijaya Dairy was validated the QA way — I wrote the code AND stress-tested the edge cases.

---

## 🎓 Education & Certifications

**B.Tech — Computer Science & Engineering** · Vishnu Institute of Technology *(2020–2024)* · **CGPA: 8.19**

<div align="center">

[![Java](https://img.shields.io/badge/Java%20Certified-HackerRank-2EC866?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/20pa1a05d2)
[![SQL](https://img.shields.io/badge/SQL%20Basic%20%26%20Intermediate-HackerRank-2EC866?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/20pa1a05d2)
[![Python](https://img.shields.io/badge/PCAP%20Python-CISCO-1BA0D7?style=flat-square&logo=cisco&logoColor=white)](https://www.cisco.com)

</div>

---

## 📈 GitHub Stats

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=pulagoru-dhanush-kumar&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0d1117" />
<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=pulagoru-dhanush-kumar&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=pulagoru-dhanush-kumar&theme=tokyonight&hide_border=true&background=0d1117" />

</div>

---

## 🎯 What I'm Building Next

- [ ] 🔄 GitHub Actions CI/CD pipeline (auto deploy on push)
- [ ] 🔐 Two-Factor Authentication (2FA)
- [ ] 🌍 Custom domain + HTTPS/SSL (AWS Certificate Manager)
- [ ] 📊 Admin analytics dashboard
- [ ] ☁️ Docker + Kubernetes containerization
- [ ] 📱 React Native mobile app

---

## 🔗 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhanush-kumar-840242212/)
[![Portfolio](https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white)](https://pulagoru-dhanush-kumar.github.io/Protfolio/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/pulagoru-dhanush-kumar)
[![HackerRank](https://img.shields.io/badge/HackerRank-2EC866?style=for-the-badge&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/20pa1a05d2)
[![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black)](https://www.leetcode.com/20pa1a05d2)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](https://mail.google.com/mail/?view=cm&to=dhanushvip1729@gmail.com)

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer" />

**⭐ Star the repo if you find the project useful!**
*Java Backend Developer | Spring Boot | AWS | Open to Opportunities*

</div>
