
# Study Hub

A full-featured **study management web app** built with **HTML, TailwindCSS, Firebase, and ShowdownJS**.  
Includes **flashcards, notes, schedule, tasks, achievements, and a Pomodoro timer**.

---

## 🚀 Features
- 📚 Flashcards with spaced repetition (create, review, import/export)
- 📝 Notes with Markdown support (summarize & expand with AI placeholders)
- 📅 Weekly schedule planner with progress tracking
- ✅ Task manager with completion tracking
- ⏳ Pomodoro study timer with sound presets
- 🏆 Achievements (streaks, milestones, first deck/note, etc.)
- 🔑 Firebase authentication (Google, Email/Password, Anonymous fallback)
- ☁️ Firebase Firestore for data persistence
- 🎨 Responsive UI with TailwindCSS

---

## 📂 Project Structure
- `studyhub_complete.html` → Main app file (single-page app)
- Firebase is used for authentication & database (Firestore)
- TailwindCSS (via CDN) handles styling
- ShowdownJS is used for Markdown rendering

---

## ⚡ Getting Started

### 1. Clone or Copy the Project
```bash
git clone https://github.com/your-username/studyhub.git
cd studyhub
```

Or just copy the `studyhub_complete.html` file.

### 2. Setup Firebase
1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new Firebase project
3. Enable **Authentication** → (Google, Email/Password, Anonymous)
4. Enable **Firestore Database**
5. Go to **Project Settings → SDK Setup & Configuration**
6. Copy your Firebase config (API key, projectId, etc.)

### 3. Configure the App
Inside your `studyhub_complete.html`, replace the placeholder config:
```js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

### 4. Run Locally
Simply open the `studyhub_complete.html` file in your browser.  
Or serve it with a local web server:
```bash
npx serve .
```

### 5. Deploy Online
#### Firebase Hosting
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

#### Or Deploy to Netlify / Vercel
Just drag & drop the HTML file (Netlify) or connect your repo (Vercel).

---

## 🔧 Customization
- Update UI via Tailwind classes in the HTML.
- Extend AI functions (`generateCardsWithAI`, `summarizeNote`, `expandNote`) by connecting to an AI API (OpenAI, Claude, Gemini, etc.).
- Modify achievements logic in `checkAndAwardAchievements()`.

---

## 🛠️ Tech Stack
- **Frontend:** HTML, TailwindCSS, ShowdownJS
- **Backend:** Firebase Authentication + Firestore
- **Deployment:** Firebase Hosting / Netlify / Vercel

---

## 📜 License
MIT License © 2025
