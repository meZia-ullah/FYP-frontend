# 🧩 Frontend – Bug Severity Prediction Web Application

This is the **React.js frontend** of the Final Year Project:  
🎓 **"An Automated Approach for the Prediction of the Severity Level of Bug Reports Using LLMs"**

The interface allows users to input bug reports and view the predicted severity level powered by a backend AI model based on Large Language Models (LLMs) like XLNet.

---

## 🎯 Objective

To provide an intuitive web interface for developers and QA engineers to:
- Submit bug report text
- Automatically predict severity level (e.g., Critical, Major, Minor, Trivial, etc.)
- Improve issue triaging and bug report prioritization using AI

---

## 🧰 Technologies Used

| Category           | Tools / Libraries                      |
|--------------------|-----------------------------------------|
| Frontend Framework | [React.js](https://reactjs.org)        |
| Styling            | Tailwind CSS or Bootstrap              |
| HTTP Client        | [Axios](https://axios-http.com)        |
| State Handling     | React Hooks (`useState`, `useEffect`)  |
| Environment Config | `.env`                                 |
| Build Tool         | Create React App (CRA)                 |

---

## 🚀 Features

- 📝 Submit bug report through a clean text input interface
- 📊 View predicted severity level and confidence score
- 🔗 Communicate with backend API for model inference
- ⏳ Show loading indicator during prediction
- ⚠️ Graceful error handling for API failures
- 📱 Fully responsive and mobile-friendly design

---

## 📸 Screenshots

![Screenshot 2025-05-18 124104](https://github.com/user-attachments/assets/470c6621-a4d0-4f77-968a-6b26a7bf0fc4)


---

## 📦 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/your-repo-name.git
cd frontend
```

### 2. Install dependencies
```bash
npm install
```

### 3. Create `.env` file
Add the following to a file named `.env` in the `frontend/` directory:
```
REACT_APP_API_URL=http://localhost:5000/api/predict
```

> Change the URL if your backend is hosted remotely.

### 4. Start the development server
```bash
npm start
```

Then open your browser at: [http://localhost:3000](http://localhost:3000)

---

## 🔗 API Integration

The frontend sends a `POST` request to the backend server:

### Endpoint
```
POST /api/predict
```

### Request Body
```json
{
  "bug_report": "App crashes when the user clicks the login button."
}
```

### Sample Response
```json
{
  "severity": "Critical",
  "confidence": 0.94
}
```

---

## 📁 Folder Structure

```
frontend/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   └── BugInputForm.js
│   │   └── PredictionResult.js
│   ├── pages/
│   │   └── Home.js
│   ├── App.js
│   ├── index.js
├── .env
├── package.json
└── README.md
```

---

## 🔒 Best Practices Followed

- Separation of concerns: components/pages structure
- Environment variable for backend URL
- Proper loading and error states for better UX
- Axios used for HTTP requests with clean abstraction

---

## 📌 Future Enhancements

- User authentication and bug history
- Confidence percentage visualized via progress bars or charts
- Dark/light theme toggle
- Multi-language support (i18n)


---

## 👨‍💻 Authors

- **Zia Ullah** – AI Model, Backend Development
- **Saad Saeed** – Frontend Development, UI/UX

Final Year Project – BS Software Engineering  
Department of Information Technology
University of Haripur

---

