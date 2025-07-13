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

#### 📸 Daily Standups & Retrospective  
![Daily Stand](https://github.com/user-attachments/assets/353a3179-dc4a-4c5d-b067-0f263b29fe24)
![Retrospective](https://github.com/user-attachments/assets/4952f5d3-e204-44dc-a426-cf66aaf0c82b)

### 2️⃣ Database Design  
- Designed full **ERD** for `Examination_OLTP`  
![ERD drawio](https://github.com/user-attachments/assets/218f1c6e-728e-4517-b8ee-a379e0bd13a0)
![OLTP_Diagram](https://github.com/user-attachments/assets/3e9f3398-3876-41ec-afae-5350f83a490d)
- Created Galaxy Schema for `Examination_OLAP`  
![OLAP Model](https://github.com/user-attachments/assets/24059892-588e-4442-803c-5ae959f9d9d8)
- Documented mapping between transactional and analytical layers  
![Final Mapping](https://github.com/user-attachments/assets/c395d235-14dd-45a6-aad9-52310b0155a9)

### 3️⃣ ETL & Reporting Tools  
- **SSIS** for ETL from OLTP to OLAP  
![fact instructor evaluation](https://github.com/user-attachments/assets/1e7f63d9-2f3c-4843-91a8-066bcdec5938)
![fact student certificate](https://github.com/user-attachments/assets/1d2b1c21-011d-4daa-92f7-95fa53195cc1)
![fact student answer](https://github.com/user-attachments/assets/41704ba6-ddd6-4c9c-8e9a-595a748033d0)
![Dim Student](https://github.com/user-attachments/assets/9090f084-5715-437f-a82b-8210ea0d2dd1)
![Dim instructor](https://github.com/user-attachments/assets/3f5e85c7-c297-4153-803f-1b846d724cf9)

- **SSAS** for cube building  
- **SSRS** for paginated reports and analytics  
![SSRS 1](https://github.com/user-attachments/assets/4abcb9c0-70ab-47e4-bbcc-dd7999cda24a)
![SSRS 2](https://github.com/user-attachments/assets/cdddd3ab-6530-48c5-bed1-2124bec2d8a9)
![SSRS 3](https://github.com/user-attachments/assets/76d4a2c1-a190-4895-8a82-3a4432197543)
![SSRS 4](https://github.com/user-attachments/assets/dc8863dd-a0c5-4886-b635-69d96b59ee0c)
![SSRS 5](https://github.com/user-attachments/assets/ebd44c23-9190-4cb4-b217-cb8cffbcc944)

### 4️⃣ Dashboards & Analytics  
- Developed 25+ dashboards using **Power BI**
- ![Instructor](https://github.com/user-attachments/assets/77773f33-3aca-4b41-a70f-f138cf3c3b06)
- ![Instructor 2](https://github.com/user-attachments/assets/33cb0499-2497-44f8-980e-b5de91fa3344)
- ![Instructor 4](https://github.com/user-attachments/assets/10221c51-980e-428d-9444-04dce530b05c)
-![branch 2](https://github.com/user-attachments/assets/64047fed-8fc6-4a14-95e4-5d96e2a80ae1)
- ![Branch](https://github.com/user-attachments/assets/18575134-ac91-4421-935c-743b757687a5)
- ![student per branch](https://github.com/user-attachments/assets/b7b5f067-2eae-4cad-87b1-fdebc2ea3e79)
- Integrated **Facebook API** to track student engagement
- ![API](https://github.com/user-attachments/assets/2e6e6c94-a423-4875-a5bf-251f74d80701)

- Exportable insights via Excel and Tableau
- ![Tbleaue 1](https://github.com/user-attachments/assets/6ba7733a-0c23-494c-9cc8-716a7f119c82)

- ![Tableaue 2](https://github.com/user-attachments/assets/7801ac10-341e-4e7e-b6f5-f36d62c03248)

- <img width="567" height="719" alt="1" src="https://github.com/user-attachments/assets/b79a405c-57cb-45f0-889d-1e3730f56f70" />

- <img width="560" height="724" alt="2" src="https://github.com/user-attachments/assets/7067a51c-bb30-4f1a-9687-0caa3de02f97" />

- <img width="564" height="726" alt="3" src="https://github.com/user-attachments/assets/a1be37b7-b35d-4f7e-8b95-21616378ad48" />



### 5️⃣ Gen AI Assistant  
- Offline AI assistant using **SQLCoder-7B (gguf)**  
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/4e83d02f-d56b-4f6b-a419-e09fbe0b043b" />

<img width="1920" height="1080" alt="2" src="https://github.com/user-attachments/assets/f3c13dc2-4cc2-4d36-9426-b6e4d5763f16" />

<img width="1920" height="1080" alt="3" src="https://github.com/user-attachments/assets/1dc51fb3-6473-43e6-aa09-4543c5992def" />



- 3 Modes:  
  - **SQL Mode**: Natural Language → SQL  
    ![SQL Mode](https://github.com/user-attachments/assets/201933fe-b92e-46b6-82c1-d8823cf4c19a)
  - **Chat Mode**: General Assistant  
    ![Chat Mode](https://github.com/user-attachments/assets/9f4037b5-e16d-4a2a-a765-b9924caf0339)
  - **Insight Mode**: Schema Optimization Tips  
    ![Insight Mode](https://github.com/user-attachments/assets/1a2ca7c0-5f0f-4ae9-8296-261fa0253fd0)

### 6️⃣ Web Interface  
- Dynamic web UI using **React** and **Tailwind CSS**  
- Seamless access for students, instructors, and managers  
- OLTP-integrated backend and Gen AI interface
- <img width="1861" height="912" alt="download" src="https://github.com/user-attachments/assets/c5d404b3-c2f8-4d91-bdb1-54e9287bbc75" />

- <img width="1920" height="861" alt="download (2)" src="https://github.com/user-attachments/assets/98d1ef70-528e-4cee-a150-0e621ca39071" />

- <img width="1915" height="870" alt="Admin" src="https://github.com/user-attachments/assets/55f08979-4911-4f24-8460-1518ebf197e3" />

- <img width="1920" height="940" alt="Register" src="https://github.com/user-attachments/assets/1b85512e-9b61-4503-a6ff-5eb8b331374c" />





---

## 🖼️ Project Process Diagram  
![Project Process](https://github.com/user-attachments/assets/e9752ebc-4036-4668-a757-ae4c3af29467)

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
```

