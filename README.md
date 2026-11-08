# MediExplain AI

**An AI-Based Smart Medical Report Explanation System**

MediExplain AI is an AI-powered web application that helps patients understand their medical reports. A user uploads a report (PDF or image), and the system extracts the test results with OCR, checks them against normal reference ranges, and explains each result in simple, everyday language.

---

## Team Information

| | |
|---|---|
| **Team Name** | CSE4104-7D-T02 |
| **Section** | 7D |
| **Course** | CSE4104 |
| **Project Title** | MediExplain AI: An AI-Based Smart Medical Report Explanation System |
| **Team Leader** | Md Eliyas Hossain |
| **Institution** | Northern University of Business and Technology, Khulna |
| **Course Teacher** | Md. Riaz Mahmud, Assistant Professor, Dept. of CSE |

| No. | Member Name | Student ID | Role |
|---|---|---|---|
| 1 | Md Eliyas Hossain | 11230321331 | Team Leader |
| 2 | Sanjana Rahman | 11230321351 | Member |
| 3 | Md Shazzad Hossain Sayket | 11230121164 | Member |
| 4 | Mehrab Talha | 11230121206 | Member |

---

## Project Description

### Problem
Medical reports (blood tests, lipid profiles, urine tests) are full of technical terms, abbreviations and numeric values that most patients cannot interpret. Patients often wait days for a doctor's appointment, or search the internet and get confusing, inaccurate or frightening information. This causes anxiety, delayed action on abnormal results, and exposure to misinformation, especially for elderly users and people without a medical background.

### Why existing solutions are not enough
- **General AI chatbots** are not built for medical reports, give no structured result view and keep no organized report history.
- **Symptom checkers** work from typed symptoms, not from the user's actual report.
- **Educational websites** are static and do not explain a user's own results.

### Why AI is needed
- **OCR and NLP** read reports that come in many formats and layouts, which fixed rules cannot handle.
- A **Large Language Model** turns medical terminology into plain, personalized explanations and answers follow-up questions.
- Results are available instantly, any time of day, helping users prepare better for doctor visits.

### How it works
1. The user uploads a medical report (PDF or image).
2. OCR extracts the text from the report.
3. A parser identifies test names, values and units.
4. Range comparison flags each value as High, Low or Normal.
5. The OpenAI API generates a plain-language explanation from the extracted data.
6. Results, chat and history are saved in MongoDB.

### Objectives
- Convert an uploaded medical report into structured test data using OCR.
- Compare each value with its reference range and mark it High, Low or Normal.
- Generate simple test-by-test explanations and an overall summary.
- Provide an AI chat assistant for follow-up questions about the user's own report.
- Suggest questions to ask the doctor, without giving a diagnosis.
- Protect user privacy with secure accounts and a private report history.

### Expected Outcome
Users get a clear understanding of their results, less anxiety, better-prepared doctor visits and an organized history of their reports, all in one workflow instead of waiting or searching the web.

---

## Proposed Features

- **User authentication:** registration and login, with private data per user
- **Secure report upload:** PDF, JPG and PNG with file type and size validation
- **OCR text extraction:** test names, values, units and reference ranges
- **Range comparison:** automatic High / Low / Normal flags with highlighting
- **AI explanation:** plain-language explanation per test and an overall summary
- **AI chat assistant:** follow-up questions answered in the context of the report
- **Doctor-visit guide:** suggested questions and general health-awareness tips
- **Report history and dashboard:** saved reports and explanations per user
- **Safety layer:** medical disclaimer, no diagnosis or medication advice, prompt to consult a doctor for abnormal results

---

## Technology Stack

| Layer | Technology |
|---|---|
| **Frontend** | Next.js (React) |
| **Backend** | Node.js + Express.js (REST API, authentication, file handling) |
| **Database** | MongoDB |
| **AI Integration** | OpenAI API (explanations and chat) |
| **OCR** | Tesseract / Google Cloud Vision |
| **Deployment** | Vercel (frontend), Render (backend), MongoDB Atlas |

---

## Project Structure

```
CSE4104-7D-T02-MediExplain-AI/
├── client/      # Next.js frontend
├── server/      # Express.js backend (API, auth, OCR and AI services)
├── docs/        
└── README.md
```

## Getting Started

Setup and run instructions will be added as development progresses.

---

**Disclaimer:** MediExplain AI is an educational tool. It does not replace a doctor's diagnosis or treatment advice.
