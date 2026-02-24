#  Telecom Subscription System – SQL Project

**End-to-End Telecom Database | Business KPIs | ITI Project**

---

## 🏗 Project Overview

This project simulates a real-world **Telecommunication Subscription System** built using **Microsoft SQL Server**.

The system manages:
- Customers and SIM cards  
- Service plans and subscriptions  
- Usage tracking (Calls, SMS, Data)  
- Payments and extra charges  
- Complaints handling  
- Operational and business analytics  

The project combines **database design, performance optimization, and business intelligence** to reflect real telecom business scenarios.

---

## 🎯 Business Objectives

- Monitor customer activity and engagement  
- Detect **over-usage and potential churn risks**  
- Analyze **revenue performance**  
- Evaluate **service plan profitability**  
- Measure **customer acquisition and retention**  
- Track operational performance (complaints and employees)

---

## 🧩 System Modules

### Customer & SIM Management
- Customer registration
- SIM assignment to customers
- Customer activity tracking

### Subscription & Plans
- Service plan selection
- Subscription lifecycle management (Active / Suspended / Cancelled)
- Automatic payment generation

### Usage Monitoring
- Track Minutes, SMS, and Data usage
- Identify:
  - Over-limit subscriptions
  - Low remaining balance customers

### Complaints Management
- Assign complaints to employees
- Analyze employee workload
- Identify customers with repeated complaints

---

## 📊 ERD & Database Design

<details>
<summary>Click to view diagrams</summary>

### Entity Relationship Diagram
![ERD](./Diagrams/Project%20ERD%20(7).jpg)

### Mapping (Logical Schema)
![Mapping](./Diagrams/Telecom%20Mapping.drawio.png)

</details>

**Core Entities**
- Customers  
- SIM_Card  
- ServicePlan  
- Subscription  
- Usage_Records  
- Payment  
- Complaint  
- Employee  
- Department  

---

## ⚙ SQL Implementation

### Functions (Business Calculations)
- Get service plan price  
- Determine subscription status  
- Total usage (Minutes / SMS / Data)  
- Remaining usage  
- Over-limit detection   
- Subscription duration  
- Total revenue per subscription  

---

### Views (Analytics Layer)
- **Active Subscriptions**  
- **Over-Usage Monitoring**  
- **Invalid Usage Detection**  
- **Payment Summary**

These views support reporting and dashboard creation.

---

### Stored Procedures (KPIs)

#### Customer KPIs
- Active Customers Count  
- New Customers per Month  
- Idle Customers  
- Average Activation Delay  

#### Revenue KPIs
- Monthly Revenue  
- ARPU (Average Revenue Per User)  
- Revenue by Plan  
- Lost Revenue (Churn Impact)

#### Usage KPIs
- Average Usage per Plan  
- Over-Usage Rate  
- Zero Usage Subscriptions  

#### Complaints KPIs
- Complaints per Month  
- Complaints per Employee  
- Customers with repeated complaints  

---

### Triggers
Automation rules implemented:
- Automatically create payment when a subscription is activated
- Enforce business logic at the database level

---

### Performance Optimization

Indexes created on:
- `Customers(national_id)`
- `Usage_Records(subscription_id)`
- `Subscription(status)`
- `SIM_Card(CustomerID)`
- `Payment(subscription_id)`

---

### Cursors

Operational monitoring tasks:
- Identify subscriptions with extra charges
- Generate warnings for low remaining usage
- Percentage-based usage alerting

---

## 🛠 Technologies Used

- Microsoft SQL Server  
- T-SQL  
- Database Design (ERD & Normalization)  
- Performance Tuning  
- Business KPI Modeling  

---

## 👨‍💻 Author

**Mohamed Atef**  
ITI Trainee – Database / Data Track





