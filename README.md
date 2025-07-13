# 🎓 ITI Examination System

A comprehensive platform for managing exams, tracking student performance, evaluating instructors, and generating insights — all powered by databases, dashboards, and a local Gen AI assistant.

---

## 📌 Project Summary

The ITI Examination System was built for the **Information Technology Institute (ITI)** to streamline all exam-related processes, analytics, and automation across branches and departments.

It includes:
- ✅ OLTP + OLAP Databases
- ✅ SSIS-based ETL pipelines
- ✅ Power BI dashboards
- ✅ Offline Gen AI Assistant (SQLCoder-7B)
- ✅ Web Portal for Students, Instructors, Admins
- ✅ Facebook API Integration for student engagement analytics

---

## 🔄 Project Process

The project was executed in six major Agile-based phases:

### 1️⃣ Requirements & Planning  
- Defined project scope and system requirements  
- Developed a professional **SRS Document**  
- Planned sprints and user stories in **Notion**  
- Set up version control with **GitHub**

### 2️⃣ Database Design  
- Designed full **ERD** for `Examination_OLTP`  
- Created Galaxy Schema for `Examination_OLAP`  
- Documented mapping between transactional and analytical layers

### 3️⃣ ETL & Reporting Tools  
- **SSIS** for ETL from OLTP to OLAP  
- **SSAS** for cube building  
- **SSRS** for paginated reports and analytics

### 4️⃣ Dashboards & Analytics  
- Developed 25+ dashboards using **Power BI**  
- Integrated **Facebook API** to track student engagement  
- Exportable insights via Excel and Tableau

### 5️⃣ Gen AI Assistant  
- Offline AI assistant using **SQLCoder-7B (gguf)**  
- 3 Modes:  
  - **SQL Mode**: Natural Language → SQL  
  - **Chat Mode**: General Assistant  
  - **Insight Mode**: Schema Optimization Tips

### 6️⃣ Web Interface  
- Dynamic web UI using **React** and **Tailwind CSS**  
- Seamless access for students, instructors, and managers  
- OLTP-integrated backend and Gen AI interface  

---

## 🖼️ Project Process Diagram  
![Process Overview](documentation/project_process.png)

---

## 🧠 Key Features

| Feature               | Description                                                       |
|----------------------|-------------------------------------------------------------------|
| Exam Management       | Students submit answers, view results                             |
| Instructor Evaluation | Students evaluate instructors per course (0–5 scale)              |
| Dashboards            | 25+ Power BI dashboards for students, branches, intakes           |
| Gen AI Assistant      | Offline AI modes: SQL, Chat, and Insight                          |
| Facebook API          | Tracks student social engagement on ITI-related content           |
| Web Portal            | Interfaces for students, instructors, and admins                  |

---

## ⚙️ Tech Stack

- **Database**: Microsoft SQL Server (OLTP + OLAP)
- **ETL**: SSIS
- **Reporting**: SSRS, SSAS
- **BI Tools**: Power BI, Excel, Tableau
- **AI Assistant**: Python, Streamlit, ctransformers, SQLCoder-7B (gguf)
- **Frontend**: React.js + Tailwind CSS
- **Backend**: pyodbc, API integration
- **Authentication**: Windows Authentication
- **Other Tools**: Notion, GitHub

---

## 🗂️ Project Structure

```bash
ITI-Examination-System/
├── README.md
├── LICENSE
├── .gitignore
│
├── documentation/
│   ├── SRS_Document.docx
│   ├── ERD.png
│   ├── Galaxy_Schema.png
│   ├── Architecture_Diagram.png
│   └── project_process.png
│
├── database/
│   ├── Examination_OLTP.sql
│   ├── Examination_OLAP.sql
│
├── genai-assistant/
│   ├── app.py
│   ├── model/
│   │   └── sqlcoder-7b-2.Q4_K_M.gguf
│   ├── requirements.txt
│
├── web-interface/
│   ├── frontend/
│   └── backend/
│
├── powerbi/
│   └── Dashboards.pbix
│
├── ssis/
│   ├── ETL_Packages.dtsx
│
└── facebook-api/
    └── fb_api_integration.py
