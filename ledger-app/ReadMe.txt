# 🌸 Ledger — Tasks, Habits, Diary & Insights

Ledger is a beautiful, minimalist, and lightweight personal dashboard designed to track your daily discipline. Built as a single-file web application, it brings together task management, a dynamic weekly habit schedule, an event reminder system, a personal diary, and a visual commitment heatmap—all powered by a real-time serverless backend.

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)

---

## ✨ Features

* **📝 Smart Task Manager:** Create, prioritize (High/Medium/Low), and schedule tasks with due dates. Active tasks persist on your weekly schedule until completed.
* **📅 Dynamic Weekly Schedule & Habits:** Track recurring habits with active day selections. Log daily completions and view real-time habit streaks.
* **🔔 Events & Reminders:** Set up event timelines with optional real-time browser push notifications.
* **📔 Private Diary:** Record thoughts, notes, and logs day-by-day.
* **💫 Insights & Analytics:** * 30-day task completion rate metrics.
    * 30-day habit consistency gauges.
    * An interactive **14-week visual consistency map** (GitHub-style contribution heatmap) tracking overall daily engagement.
* **🔒 Secure Multi-User Auth:** Complete email-and-password sign-up and login gates handled seamlessly via serverless authentication.

---

## 🛠️ Architecture & Tech Stack

* **Frontend:** Pure Semantic HTML5, CSS3 Custom Properties (Gradients & Variables), JavaScript (ES6+ Vanilla).
* **Fonts:** `Quicksand` & `Baloo 2` via Google Fonts.
* **Backend Database & Auth:** [Supabase](https://supabase.com/) (PostgreSQL & GoTrue Auth Engine via CDN client client package).

---

## 🚀 One-Time Local Setup

Because Ledger runs as a zero-build client-side app, setting it up takes under two minutes:

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd YOUR_REPO_NAME
    ```

2.  **Configure Your Backend:**
    * Create a free project over at [Supabase](https://supabase.com/).
    * Navigate to **Project Settings > API** to find your `Project URL` and `Anon Key`.
    * Open `ledger-hosted.html` (or `index.html`) in a code editor and replace the configuration placeholders near the top of the `<script>` section:
    ```javascript
    // ====================== FILL THESE IN FROM YOUR SUPABASE PROJECT ======================
    const SUPABASE_URL = 'YOUR_SUPABASE_PROJECT_URL';
    const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_KEY';
    // =======================================================================================
    ```

3.  **Database Tables Required:**
    Ensure your Supabase project contains the corresponding schemas for `tasks`, `habits`, `diary_entries`, and `events` tables mapping your local row fields.

4.  **Run:**
    Simply double-click the HTML file to open it in any modern browser, or spin up a local server using VS Code's *Live Server* extension!

---

Manage your day with ledger and help others too...