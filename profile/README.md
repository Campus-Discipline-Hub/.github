# 📘 CampusDiscipline Hub – Smart Discipline Management System  

![Status](https://img.shields.io/badge/Status-In%20Progress-yellow)
![Version](https://img.shields.io/badge/Version-1.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Repo Size](https://img.shields.io/github/repo-size/Campus-Discipline-Hub/Discipline-Management-System)
![Contributors](https://img.shields.io/github/contributors/Campus-Discipline-Hub/Discipline-Management-System)
![Forks](https://img.shields.io/github/forks/Campus-Discipline-Hub/Discipline-Management-System?style=social)
![Stars](https://img.shields.io/github/stars/Campus-Discipline-Hub/Discipline-Management-System?style=social)
![Pull Requests](https://img.shields.io/github/issues-pr/Campus-Discipline-Hub/Discipline-Management-System)
![Last Commit](https://img.shields.io/github/last-commit/Campus-Discipline-Hub/Discipline-Management-System)
![HTML5](https://img.shields.io/badge/Frontend-HTML5-orange?logo=html5)
![CSS3](https://img.shields.io/badge/Frontend-CSS3-blue?logo=css3)
![JavaScript](https://img.shields.io/badge/Frontend-JavaScript-yellow?logo=javascript)
![Chart.js](https://img.shields.io/badge/Analytics-Chart.js-pink?logo=chartdotjs)
![XAMPP](https://img.shields.io/badge/Backend-XAMPP-F37623?logo=xampp&logoColor=white)


## 👥 Contributors

<a href="https://github.com/Campus-Discipline-Hub/Discipline-Management-System/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Campus-Discipline-Hub/Discipline-Management-System" />
</a>

## 📌 Project Overview  
The **Discipline Management System** is a digital solution designed for **colleges and institutions** to monitor, record, and analyze student discipline activities.  
It ensures a **transparent workflow** between Mentors, Advisors, Year In-charge, Department Discipline In-charge, HODs, Dean, Principal, and the **Overall Discipline Head**.  

---

## 📖 Introduction  
**CampusDiscipline Hub** is a centralized **Discipline Management System** designed for colleges.  
It provides a **transparent, structured, and digital workflow** to handle both **normal discipline issues** and **high-alert cases**, ensuring accountability and efficiency across different roles (Faculty, Mentors, HODs, Dean, Principal, Discipline Head).  

---

## 🎯 Objectives  
- Maintain a **structured digital record** of discipline cases  
- Provide **transparent access** to stakeholders based on hierarchy  
- Escalate repeated misconduct cases with **clear workflows**  
- Minimize **manual paperwork & errors**  
- Enable **data-driven insights** into student behavior patterns  

---

## ⚡ Key Features  
### Normal Issues  
- Report entry by **Year/Department In-charge**  
- Accessible by **Mentor, Advisor, HOD, Dean, Principal, Discipline Head**  
- Case closure only by **Year/Department In-charge** (post verification)  
- Letter upload & approval process for resolution  

### High Alert Issues  
- Direct entry by **Discipline Head**  
- Full authority to **view/add/download**  
- Senior management (HOD, Dean, Principal) can **view/download only**  
- Mentors/Advisors/In-charges have **view-only** access  

---

## 🗂 Data Management  

### **Base Table Fields**  
- `Reg No`, `Name`, `Year`, `Dept`  
- `Entry Date`, `Reason`, `Status`, `Close Date`  
- `Occurrence`, `Mentor`, `Advisor`  

### **Access Control**  
- **DDI/YI** → File upload, action taken  
- **Mentor/Advisor** → View only  
- **Discipline Head** → Full authority on critical cases  

---

## 💻 Tech Stack  

- **Frontend** → HTML5, CSS3, JavaScript  
- **Data Storage** → LocalStorage (Future: SQLite/MySQL)  
- **Analytics** → Chart.js  
- **Future Expansion** → Flask/Node.js backend, ERP integration, Mobile App  

---

## ✨ Benefits  
✔ Transparent record of discipline actions  
✔ Prevents repeated misconduct with escalation rules  
✔ Saves time with structured digital workflow  
✔ Enables long-term data analysis  
✔ Reduces paper usage & manual errors  

---

## 🚀 Future Scope  
📩 **Parent Notification System** (SMS/Email)  
📱 **Mobile App version**  
🤖 **AI/ML-based discipline pattern prediction**  
🔗 **ERP/Cloud integration**  

---

## 🏗️ System Hierarchy  

**Principal → Dean → HOD → Discipline Head → Year In-charge / Department In-charge → Student Mentor/Advisor → Students**  

## 📊 Workflow (Mermaid Diagram)

```mermaid
flowchart TD
    P[👨‍🏫 Principal] --> D[📘 Dean]
    D --> H[🏛 HOD]
    H --> DH[⚖ Discipline Head]
    DH --> YI[📂 Year In-charge / Dept In-charge]
    YI --> M[👨‍💼 Mentor / Advisor]
    M --> S[🎓 Student]

    %% Escalation Paths
    S -->|Misconduct Case| YI
    YI -->|Escalation| DH
    DH -->|Critical Case| P

