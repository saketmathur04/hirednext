
# 🚀 hiredNext - AI-Powered Mock Interview Platform

![Project Banner](/public/logo.png)

Practice job interviews with AI-powered feedback and land your dream job! 💼 Powered by cutting-edge AI from Vapi and Google Gemini.

---

## 🌟 Features

- **🔐 Auth System**: Secure sign-up/login with Firebase Authentication
- **🤖 AI Interview Generation**: 
  - Customize interviews by role, tech stack & difficulty
  - Get instant AI-generated questions
- **🎙️ Real-time Practice**:
  - Interactive voice-based interviews
  - AI interviewer with natural conversation flow
- **📊 Smart Feedback**:
  - Detailed performance reports
  - Category-wise scoring (Technical, Communication, etc.)
  - Strengths & improvement areas
- **📈 Dashboard**:
  - Track interview history
  - Retake interviews

---

## 🛠️ Tech Stack

- **Framework**: Next.js 15 (App Router)
- **Database**: Firebase Firestore
- **Auth**: Firebase Authentication
- **AI Services**:
  - Vapi.ai (Voice AI)
  - Google Gemini (Question Generation & Feedback Analysis)
- **Styling**: Tailwind CSS + Shadcn UI
- **State Management**: React Hook Form
- **Utilities**: Day.js, Zod

---

## 🚀 Getting Started

### Prerequisites

- Node.js v18+
- Firebase project
- Vapi.ai & Google Gemini API keys

### Installation

1. **Clone the repository**:
```bash
git clone https://github.com/abdullah0408/hirednext-mock_interviewing_platform.git
cd hirednext-mock_interviewing_platform
```

2. **Install dependencies**:
```bash
npm install --legacy-peer-deps
```

3. **Set up environment variables**:

Create a `.env.local` file in the root and add:

```env
FIREBASE_PROJECT_ID=
FIREBASE_PRIVATE_KEY=
FIREBASE_CLIENT_EMAIL=
GOOGLE_GENERATIVE_AI_API_KEY=

NEXT_PUBLIC_VAPI_WEB_TOKEN=
NEXT_PUBLIC_VAPI_WORKFLOW_ID=
```

---

## 🔧 Firebase Setup

Before running the project, you need to connect it with your own Firebase project.

1. Go to the [Firebase Console](https://console.firebase.google.com/)
2. Create a new project (or use an existing one)
3. Navigate to **Project Settings → General → Add App → Web App**
4. Copy the provided Firebase config

Now, open `firebase.ts` (or `firebase.js`) and **replace the placeholder config** with your own:

```ts
// firebase/client.ts

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID",
  measurementId: "YOUR_MEASUREMENT_ID", // optional
};
```

> ⚠️ **Note**: Do **not** use the Firebase config from this repo — it's specific to the project creator and may result in errors or security issues.

Also make sure you've set up Firebase Authentication and Firestore in your Firebase project.

---

### Run Development Server

```bash
npm run dev
```

App will be running locally at [http://localhost:3000](http://localhost:3000)

---

## 🎯 Usage

1. **Sign Up** ➡️ Create a new account
2. **Generate Interview** ➡️ Choose role, tech stack, and difficulty
3. **Practice** ➡️ Voice-based interview session with AI
4. **Get Feedback** ➡️ Review your performance with detailed insights

---

## 📌 Future Improvements

- Resume parsing for personalized interviews
- Multi-language support
- Company-specific interview templates
- Leaderboard for peer comparison
