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
- [SRS_Beta.Version 1.0.docx](https://github.com/user-attachments/files/21202016/SRS_Beta.Version.1.0.docx)
- <img width="1864" height="870" alt="Daily_Stand" src="https://github.com/user-attachments/assets/353a3179-dc4a-4c5d-b067-0f263b29fe24" />
<img width="1864" height="870" alt="Retrospective" src="https://github.com/user-attachments/assets/4952f5d3-e204-44dc-a426-cf66aaf0c82b" />


### 2️⃣ Database Design  
- Designed full **ERD** for `Examination_OLTP`
- <img width="3962" height="2175" alt="ERD drawio" src="https://github.com/user-attachments/assets/218f1c6e-728e-4517-b8ee-a379e0bd13a0" /> 
-<img width="1210" height="790" alt="OLTP_Diagram" src="https://github.com/user-attachments/assets/3e9f3398-3876-41ec-afae-5350f83a490d" />
- Created Galaxy Schema for `Examination_OLAP`
- <img width="867" height="793" alt="olap model" src="https://github.com/user-attachments/assets/24059892-588e-4442-803c-5ae959f9d9d8" />
- Documented mapping between transactional and analytical layers
- <img width="1593" height="1472" alt="Final Mapping" src="https://github.com/user-attachments/assets/c395d235-14dd-45a6-aad9-52310b0155a9" />

### 3️⃣ ETL & Reporting Tools  
- **SSIS** for ETL from OLTP to OLAP
- <img width="967" height="467" alt="fact instructor evaluation" src="https://github.com/user-attachments/assets/1e7f63d9-2f3c-4843-91a8-066bcdec5938" />
<img width="1452" height="473" alt="fact student certificate" src="https://github.com/user-attachments/assets/1d2b1c21-011d-4daa-92f7-95fa53195cc1" />
<img width="1242" height="463" alt="fact student answer" src="https://github.com/user-attachments/assets/41704ba6-ddd6-4c9c-8e9a-595a748033d0" />
<img width="525" height="392" alt="Dim Student" src="https://github.com/user-attachments/assets/9090f084-5715-437f-a82b-8210ea0d2dd1" />
<img width="535" height="388" alt="Dim instructor" src="https://github.com/user-attachments/assets/3f5e85c7-c297-4153-803f-1b846d724cf9" />
- **SSAS** for cube building  
- **SSRS** for paginated reports and analytics
- <img width="826" height="767" alt="Screenshot 2025-07-12 232529" src="https://github.com/user-attachments/assets/4abcb9c0-70ab-47e4-bbcc-dd7999cda24a" />
<img width="839" height="859" alt="Screenshot 2025-07-12 232728" src="https://github.com/user-attachments/assets/cdddd3ab-6530-48c5-bed1-2124bec2d8a9" />
<img width="779" height="827" alt="Screenshot 2025-07-12 232803" src="https://github.com/user-attachments/assets/76d4a2c1-a190-4895-8a82-3a4432197543" />
<img width="767" height="798" alt="Screenshot 2025-07-13 025629" src="https://github.com/user-attachments/assets/dc8863dd-a0c5-4886-b635-69d96b59ee0c" />
<img width="599" height="801" alt="Screenshot 2025-07-13 025729" src="https://github.com/user-attachments/assets/ebd44c23-9190-4cb4-b217-cb8cffbcc944" />

### 4️⃣ Dashboards & Analytics  
- Developed 25+ dashboards using **Power BI**  
- Integrated **Facebook API** to track student engagement  
- Exportable insights via Excel and Tableau

### 5️⃣ Gen AI Assistant  
- Offline AI assistant using **SQLCoder-7B (gguf)**
-   <img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/6d6de9e2-8082-4b2a-86da-8142f67b99ed" />
-   <img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/b342f50b-5d96-4733-ac7a-786885e7f183" />

- 3 Modes:  
  - **SQL Mode**: Natural Language → SQL
  - <img width="995" height="770" alt="Mode_1" src="https://github.com/user-attachments/assets/201933fe-b92e-46b6-82c1-d8823cf4c19a" />

  - **Chat Mode**: General Assistant
  - <img width="996" height="776" alt="Mode_2" src="https://github.com/user-attachments/assets/9f4037b5-e16d-4a2a-a765-b9924caf0339" />

  - **Insight Mode**: Schema Optimization Tips
  - <img width="1000" height="781" alt="Mode_3" src="https://github.com/user-attachments/assets/1a2ca7c0-5f0f-4ae9-8296-261fa0253fd0" />

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
