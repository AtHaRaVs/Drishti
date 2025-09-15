# Drishti 👁️
![MERN](https://img.shields.io/badge/Stack-MERN-green?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![AST](https://img.shields.io/badge/AST-Analysis-blue?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)



**Drishti** is a repository comprehension engine designed to give developers **deep architectural understanding** of unfamiliar codebases.  
Unlike tools that only provide statistics or surface-level documentation, Drishti helps you answer critical questions like:

- *"How does authentication flow work in this codebase?"*  
- *"What happens when a user clicks 'submit' on the payment form?"*  
- *"Where are the database models defined and how do they relate?"*  
- *"What are the critical dependency paths I shouldn't break?"*  
- *"How is error handling implemented across services?"*  

Drishti = **Clarity into your repositories.**  

---

## ✨ Features

- 🏗️ **Architecture Understanding** – Detects architectural patterns, entry points, and data flow.  
- 🔄 **Business Logic Flows** – Extracts end-to-end flows (e.g., authentication, payment).  
- 🔍 **Cross-File Relationship Mapping** – Trace complete user journeys across files.  
- 📦 **Configuration Parsing** – Understands package.json, env vars, and dependencies.  
- ⚠️ **Impact Analysis** – Know what breaks if you modify a function.  
- 📖 **Architecture Decision Docs** – Inferred reasoning behind technical choices.  
- 🔐 **Security Analysis** – Detects auth strategies, validation, and vulnerabilities.  

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/drishti.git
cd drishti
```

### 2️⃣ Install Dependencies

#### Backend
```bash
cd server
npm install
```

#### Frontend
```bash
cd client
npm install
```

### 3️⃣ Setup Environment Variables
Create a `.env` file inside `server` with the following:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
GITHUB_TOKEN=your_github_token
JWT_SECRET=your_secret_key
```

### 4️⃣ Run the Project

#### Backend
```bash
cd server
npm run dev
```

#### Frontend
```bash
cd client
npm run dev
```

Frontend → `http://localhost:5173/`  
Backend → `http://localhost:5000/`  

---

## 📖 Example Outputs

### 🏗️ System Architecture
```
Request → API Layer → Business Logic → Data Access → Database
```

### 🔑 User Registration Flow
1. Input Validation → `src/validators/user.validator.js`  
2. Duplicate Check → `src/services/user.service.js`  
3. Password Hashing → `src/utils/crypto.js`  
4. Database Insert → `src/models/user.model.js`  
5. Email Verification → `src/utils/email.service.js`  

### ⚠️ Impact Analysis
```
Function: validatePayment
Direct Callers: processOrder, refundPayment
Indirect Impact: emailConfirmation, inventoryUpdate
Risk Level: HIGH
```

---

## 📜 License
This project is licensed under the **MIT License**.  

---

## 🙌 Acknowledgements
- Inspired by the need for **faster onboarding** into complex systems.  
- Combines learnings from RepoAgent, DeepWiki, and architectural analysis tools.  
- Built for developers who want to go beyond reading code — to **understanding systems**.  
