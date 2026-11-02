# StudyFlow — Smart Demo (TAC 101 Assignment 7, Mock Product)

## Start
Open `index.html` in Chrome, Safari, or Firefox. No installation, server, account, API key, or internet connection required. Keep all files in this folder together.

## Pages
- `index.html`: Landing Page
- `features.html`: Information Page (features and proposed pricing)
- `demo.html`: Interactive natural-language-inspired planner
- `signup.html`: Sign Up Page with email validation and confirmation (no email stored)

## Live demo walkthrough
1. Go to Live demo and choose the "Calculus midterm" example, or type your own request.
2. Select a future deadline, total hours, and available hours per day.
3. Click "Generate my study plan" to see a keyword-based task breakdown and daily study sessions.
4. Click "Complete" on a session; progress updates and remaining sessions are recalculated.
5. Click "Missed day" on a session; that date is excluded and unfinished work is redistributed.
6. Try a tight deadline with too few available hours; a capacity warning appears.
7. Visit Sign up and submit a valid email; a confirmation appears, but nothing is saved or sent.

## Honest prototype limitations
This is a rule-based demonstration, NOT a ChatGPT-like AI model. It recognizes common English and Chinese keywords for exams, programming, writing, and presentations. It offers template steps rather than dynamically reasoning about course material. It does not connect to any backend or store signup emails. The planner stores its demo state in the browser's localStorage (if permitted). Completion is tracked in study hours; a session can be completed or missed, then remaining hours are replanned. Daily capacity is shared across the single current study goal; multiple concurrent goals are not supported in this version.

## Deployment
This static site is compatible with GitHub Pages. Upload all HTML, CSS, and JS files to the repository root and enable GitHub Pages (Deploy from branch, main, root). No secrets are needed. Confirm your professor's submission format in Brightspace.

## Credits
StudyFlow concept: Zihao Cai and Yijin Wu (Assignment 6). Prototype developed with AI coding assistance; disclose AI assistance according to course rules.

## V4 personalization changes
The demo now detects subject (including Physics, Calculus, C++, Python), chapter count (e.g. 5 chapters), and selected weak topics. It creates chapter-specific tasks and attaches those tasks to daily sessions instead of repeating the user's entire prompt. It still uses deterministic rules and cannot truly reason like ChatGPT.
