# EduQuiz – Online Quiz & Assessment System

A fully functional, multi-page quiz website built with plain HTML, CSS, and JavaScript.  
No frameworks, no npm, no build step required — just open and run.

---

## 📁 File Structure

```
eduquiz/
├── login.html       ← Entry point (start here)
├── register.html    ← Registration page
├── dashboard.html   ← Quiz selection dashboard
├── quiz.html        ← Quiz taking page
├── result.html      ← Result & score summary
└── README.md        ← This file
```

---

## 🖥️ Running Locally on Your PC

### Option A — Open Directly in Browser (Simplest)
1. Download or unzip the `eduquiz/` folder to your computer.
2. Double-click `login.html` to open it in your browser.
3. Done! Navigate between pages using the login and quiz buttons.

> ⚠️ Some browsers block `sessionStorage` when opening files via `file://`. If pages redirect unexpectedly, use Option B below.

---

### Option B — Run with VS Code Live Server (Recommended)
1. Install **Visual Studio Code** → https://code.visualstudio.com/
2. Open VS Code → Go to **Extensions** (Ctrl+Shift+X) → search **"Live Server"** → Install it.
3. Open the `eduquiz/` folder in VS Code: **File → Open Folder**
4. Right-click `login.html` in the file explorer → **"Open with Live Server"**
5. Your browser will open at `http://localhost:5500/login.html`

---

### Option C — Run with Python (No install needed if Python is present)
1. Open a terminal/command prompt in the `eduquiz/` folder.
2. Run:
   ```bash
   # Python 3
   python -m http.server 3000

   # Python 2
   python -m SimpleHTTPServer 3000
   ```
3. Open your browser at → `http://localhost:3000/login.html`

---

## 🌐 Hosting on GitHub Pages

### Step 1 — Create a GitHub Account
Go to https://github.com and sign up (free).

### Step 2 — Create a New Repository
1. Click the **+** button → **New Repository**
2. Name it: `eduquiz` (or anything you like)
3. Set visibility to **Public**
4. Click **Create Repository**

### Step 3 — Upload Your Files
**Via GitHub Web UI (easiest):**
1. On your new repo page, click **"uploading an existing file"**
2. Drag and drop ALL 5 HTML files into the upload area
3. Click **"Commit changes"**

**Via Git CLI (if you have Git installed):**
```bash
cd path/to/eduquiz/
git init
git add .
git commit -m "Initial EduQuiz upload"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/eduquiz.git
git push -u origin main
```

### Step 4 — Enable GitHub Pages
1. In your repo, go to **Settings** → **Pages** (left sidebar)
2. Under **Source**, select: **Deploy from a branch**
3. Branch: **main** | Folder: **/ (root)** → Click **Save**
4. Wait ~1 minute, then your site will be live at:
   ```
   https://YOUR_USERNAME.github.io/eduquiz/login.html
   ```

> 💡 **Tip:** To make `login.html` the default page, rename it to `index.html`. Then your site will open directly at `https://YOUR_USERNAME.github.io/eduquiz/`.

---

## 🔑 How to Login (Demo Credentials)
The login is a **mock login** — any email/password combination works.  
Enter any valid-looking email and any password (1+ characters) and click LOGIN.

---

## 📝 Quiz Topics Available
| Topic | Questions | Total Points |
|-------|-----------|-------------|
| Fundamentals of Mathematics | 5 | 15 |
| Basic Sciences | 5 | 15 |
| World History Essentials | 5 | 15 |

Pass mark: **70%** or above.

---

## ✨ Features
- Responsive, mobile-friendly layout
- Progress bar on quiz page
- Animated score ring on result page
- PASS / FAIL detection (≥70% = PASS)
- Quiz history tracking (per session)
- Dashboard shows quizzes taken, last score, best result
- 3 different quiz topics

---

© 2024 EduQuiz Inc.