# NEET-Command
Your Go To Solution For NEET Mastery







NEET COMMAND CENTER
Complete User Guide

Your all-in-one NEET UG study dashboard — track chapters, rate topics,
log errors, analyse mock performance, and get an AI-powered daily plan.



Target: 720 / 720  ·  NEET UG 2026


Table of Contents
1. Getting Started
2. Setup & Configuration
3. Daily Workflow
4. All Sections Explained
5. Topic-wise Ratings & Backlogs
6. AI Study Advisor
7. Mock Test Tracker
8. Heatmap & Spaced Repetition
9. Calendar Sync
10. Chapter Notes
11. Tips to Reach 720
12. Troubleshooting

1. Getting Started
The NEET Command Center is a single HTML file that runs entirely in your browser. There is no installation, no account, and no server required. All your data is stored locally in your browser.

Opening the Tool
1	Download the HTML file
Save neet-portal.html to your computer — anywhere you like (Desktop, Documents, etc.)
2	Open in Chrome or Edge
Double-click the file to open it. Use Chrome or Edge for best compatibility. Firefox also works.
3	Bookmark it
Bookmark the file URL (e.g. file:///C:/Users/You/Desktop/neet-portal.html) so you can open it every day with one click.
4	Keep the same file
Your data is saved in the browser's localStorage for that file. Moving or renaming the file will not lose your data as long as you open it in the same browser.

💡  Do NOT open in incognito/private mode — localStorage is disabled there and your data will not save.
💡  If you use multiple computers, export your data manually (Ctrl+S to save a copy of the HTML with your localStorage intact is NOT possible — instead, note that data does not sync across devices).

2. Setup & Configuration
Before using the AI Study Advisor and Calendar Sync, you need two optional API keys. Everything else works without any keys.

Step 1 — Open Settings
→  Click ⚙ Cal Settings in the top-right of the top bar. A settings panel slides down.

Step 2 — Groq API Key (for AI Study Advisor)
The AI Study Advisor uses Groq's free API. It is completely free with 14,400 requests per day — more than enough.
    1. Go to console.groq.com/keys
    2. Sign up for a free account
    3. Click "Create API Key" and copy it
    4. Paste it into the "Groq API Key" field in settings
    5. Click Save

💡  The AI will now auto-generate your daily plan every morning. It reads your tasks, weak topics, mock errors, and backlogs to build a personalised schedule.

Step 3 — Google Calendar API Key (optional, for sync)
If you manage your study schedule and mock tests in Google Calendar, you can sync them automatically.
    6. Go to console.cloud.google.com
    7. Create a project → Enable Google Calendar API
    8. Create an API key under Credentials
    9. Paste it into "Google Calendar API Key" in settings
    10. Make your calendars PUBLIC in Google Calendar settings

💡  Calendar sync pulls today's events into Today's Targets, and upcoming mock tests into the Next Mock Test widget.

3. Your Daily Workflow
Here is the recommended sequence to get the most out of the portal every day.

1	Morning — Check Today's Targets
Open the portal. Sync your calendar (↻ Sync Cal button). Review your tasks for the day. The AI plan auto-generates in the background.
2	Morning — Review Backlogs & Revisions Due
Check the ⚠ Backlogs section for overdue topics. Check 📚 Revisions Due for spaced repetition items due today. Prioritise these before new content.
3	While Studying — Tick Chapters Done
After finishing a chapter, tick it in Subject Chapter Tracker. The topic-wise rating modal will pop up — rate every sub-topic honestly.
4	After a Mock — Log Marks & Errors
Enter your marks in Mock Test Marks Tracker immediately after each mock. The error log panel appears automatically — add every topic you got wrong.
5	Evening — Regenerate AI Plan
If you added errors or completed chapters, click ↻ Regenerate in the AI Study Advisor to get a fresh plan for tomorrow.
6	Weekly — Review the Heatmap
Check the Chapter Strength Heatmap to see your overall strength map. Any red or dark cells need immediate attention.

4. All Sections Explained
The portal is arranged top-to-bottom. Here is every section and what it does.

Section	What it does	Key actions
Hero / Top Bar	Shows today's date, Next Mock Test widget, and NEET countdown timer	Click ⚙ for settings, ↻ Sync on mock widget
Stats Bar	Chapters done, mocks taken, average score, day streak — all live	Click streak dots to mark study days
⚠ Backlogs	Topics you need to revisit — colour coded by urgency	Add manually or auto-added from weak topic ratings
📚 Revisions Due	Chapters due for spaced repetition review today	Click ✓ on a chip to mark reviewed
Today's Targets	Today's study tasks from calendar or manual entry	↻ Sync Cal, + Add, click task to toggle done
Syllabus Completion	Ring chart (overall %) and bars for Phy/Chem/Bio	Auto-updates as you tick chapters done
Chapter Heatmap	Colour grid of all 97 chapters — your strength map	Hover for chapter name, colours = rating level
Subject Chapter Tracker	Full NEET syllabus, class-wise, with stars and notes	Tick done, rate topics, add notes per chapter
AI Study Advisor	Groq-powered daily study plan with schedule + tips	Reads all your data, generates 4-block plan
Schedules	Google Calendar iframes for mock tests + study targets	Click ↗ to open in Google Calendar
Mock Marks Tracker	Enter mock scores, see trend chart and target tracker	Save mock → error log panel appears

5. Topic-wise Ratings & Backlogs
This is the most important part of the system. Rating individual topics (not just chapters) is what makes the AI advice precise.

How Topic Ratings Work
When you tick a chapter as done in the Subject Chapter Tracker, a modal automatically pops up. It lists every sub-topic in that chapter — 5 topics on average, defined specifically for NEET.
For each sub-topic you see five stars. Rate each one:

Stars	Meaning	What happens automatically
★	Very Shaky	Auto-added to backlogs due in 2 days
★★	Weak	Auto-added to backlogs
★★★	OK	Needs one more revision
★★★★	Good	Included in spaced repetition queue
★★★★★	Mastered	Blue on heatmap — you own this topic

💡  Be honest. Rating something ★★★★★ when you're actually ★★★ means the AI won't prioritise it and you'll keep losing marks on it.

What Happens After You Rate
→  ★1 and ★2 topics are automatically added to the Backlogs section with a 2-day due date.
→  The chapter's overall heatmap colour is calculated as the average of all topic ratings.
→  ★3 topics are sent to the AI as "needs one more revision" — it will schedule them.
→  ★5 topics are tracked as mastered — shown in blue on the heatmap.

Re-rating Topics
You can re-rate any topic at any time by clicking the ★ stars shown next to the chapter name in Subject Chapter Tracker (only visible for completed chapters). Click the same star again to clear a rating.

Backlog Urgency System
Backlogs are colour-coded:
    • Red glow + banner — overdue. Complete these before starting any new topics.
    • Amber — due today.
    • Dim — upcoming. Shows how many days remain.
When all backlogs are cleared, the section turns green with a ✅.

6. AI Study Advisor
The AI Study Advisor uses Groq's Llama 3.3 70B model to generate a personalised study plan. It is not generic advice — it reads your actual data.

What the AI Reads
    • Today's scheduled tasks (from calendar or manual)
    • All pending backlogs, including overdue ones
    • Every topic you rated ★1 or ★2 (very shaky / weak) — listed by specific topic name, not just chapter
    • Topics you rated ★3 (needs revision)
    • Your top recurring error topics across all mocks, ranked by frequency
    • Chapters overdue for spaced repetition review
    • The first 120 characters of your chapter notes (formulas, key concepts)
    • Your chapter completion %, streak, mock count, and average score

The 4 Output Blocks
→  ✦ Today's Priority Focus — the top 3 specific topics to fix today and why (from your weak ratings and mock errors)
→  ⏱ Recommended Schedule — hour-by-hour plan in TIME | TOPIC | TECHNIQUE format
→  📌 How to Study Each Topic — 2-3 concrete NEET techniques per topic, referencing your own notes where possible
→  💡 Strategy & Mindset — honest assessment of what is preventing 720 and what to do about it

Plan Persistence
Once generated, today's plan is saved to the browser. Refreshing the page restores it instantly. A new day triggers a fresh auto-generation (if your Groq key is saved).

💡  The more data you give the system — ratings, errors, notes — the more specific and useful the AI plan becomes. On day 1 with no data it gives generic advice. After 5 mocks and 30 chapters rated, it tells you exactly which sub-topic to spend the next 90 minutes on.

7. Mock Test Marks Tracker
Enter your mock results immediately after each test. The system calculates averages, tracks trends, and uses your error log to power the AI plan.

Entering Marks
Two entry modes:
    • Attempts mode — enter correct and wrong answers per subject. Marks calculated as (correct × 4) − wrong.
    • Direct Marks mode — enter final marks directly if you already know them.
Fill in the test name, date, and series (ALLEN, Aakash, NTA, etc.), then hit Save Mock Result.

Error Log — Log Wrong Topics Immediately
The moment you save a mock, an error log panel appears directly below the save button. This is intentional — log your wrong topics while the paper is still fresh.
    11. Type the topic/concept you got wrong (e.g. "Nernst equation", "Meiosis I stages")
    12. Select the subject (Physics, Chemistry, Biology)
    13. Press Enter or + Add
    14. Repeat for every wrong answer

💡  Log errors at the topic level, not the chapter level. "Nernst equation" is useful. "Electrochemistry" is too broad.
You can also click the ⚠ badge on any row in the history table to edit that mock's error log later.

Performance Dashboard
    • Target Score Tracker — shows your average per subject vs your target, with a gap indicator (red = below target, green = above).
    • Phy / Chem / Bio Trend Chart — SVG line chart showing your subject-wise percentage across the last 10 mocks.
    • Avg / Best / Lowest cards — overall performance summary.

Setting Your Target Score
Click ✎ Set Target in the Target Score Tracker to set your goals. Defaults are 650 total, 140 Physics, 140 Chemistry, 370 Biology. For 720/720 set all to maximum.

8. Chapter Heatmap & Spaced Repetition

Chapter Strength Heatmap
The heatmap shows all 97 NEET chapters as a colour-coded grid, split by Physics, Chemistry, and Biology.
Colour meanings:
    • Dark (almost black) — not done yet
    • Deep red — rated ★1 (very shaky)
    • Orange — rated ★2 (weak) or has recurring mock errors
    • Dark green — done but not yet reviewed
    • Medium green — rated ★3–★4 with some revisions
    • Bright green — well revised (★4)
    • Blue — fully mastered (★5)
Hover any cell to see the chapter name. The goal is to turn the entire grid blue by exam day.

Spaced Repetition
Every chapter you tick as done is added to the spaced repetition queue. The system schedules automatic review intervals:
    • After completing: Review in 1 day
    • After 1st review: Review in 3 days
    • After 2nd review: Review in 7 days
    • After 3rd review: Review in 21 days
    • After 4th review: Review in 60 days
    • After 5th review: Review in 180 days

The 📚 Revisions Due section shows all chapters due today as chips. Each chip shows the subject colour, chapter name, and how overdue it is. Click the ✓ button on a chip to mark it reviewed — it schedules the next interval automatically.
💡  If you un-tick a chapter (mark it as not done), it is removed from the spaced repetition queue entirely.

9. Calendar Sync
The portal can sync with two Google Calendars — one for Study Targets (today's tasks) and one for Mock Tests (upcoming exams).

Requirements
    • A Google Calendar API key saved in settings (see Section 2)
    • Your calendars must be set to PUBLIC in Google Calendar → Settings → Calendar Settings → Access permissions

Syncing Today's Study Tasks
Click ↻ Sync Cal in the Today's Targets section. Events from your Study Targets calendar for today are imported as tasks. The subject (Physics/Chemistry/Biology) is auto-detected from the event title.
Multi-day events show a "Day X/Y" purple badge — so a 3-day Organic Chemistry block shows Day 1/3, Day 2/3, Day 3/3 on successive days.

Syncing Mock Tests
The Next Mock Test widget in the hero syncs automatically on page load if your API key is saved. It shows the next upcoming mock with a large day countdown, plus the next 2 after that.

Manual Exam Entry
You can also add mock exams manually using the + Add Exam button in the Next Mock Test widget. These are merged with calendar events.
💡  You don't need calendar sync for the tool to work. It is optional. Everything can be added manually.

10. Chapter Notes
Every completed chapter has a 📝 Notes button. Click it to open a full notepad for that chapter. The icon turns teal when notes exist.

What to Write in Notes
    • Key formulas (e.g. Nernst equation: E = E° − (RT/nF)lnQ)
    • Exceptions and anomalies (e.g. "Pb dissolves in dilute HNO3 but not H2SO4")
    • Memory tricks and mnemonics
    • NEET PYQ patterns (e.g. "Usually asks about Lyman series wavelength range")
    • Concepts you keep forgetting

How Notes Power the AI
The AI Study Advisor reads the first 120 characters of each chapter's notes and references them in the "How to Study" block. For example, if you wrote "Nernst: E = E° − RT/nF × lnQ" in your Electrochemistry notes, the AI will say "re-derive using your noted formula E = E° − RT/nF × lnQ from scratch."
💡  Notes are especially powerful for Chemistry (reaction mechanisms, named reactions) and Biology (mnemonic lists, exception tables).

11. Tips to Reach 720
The system can track everything, but the decisions you make with that data are what actually close the gap to 720.

The Non-negotiables
    15. Rate every sub-topic the day you finish a chapter. Do not skip. This is what makes the AI useful.
    16. Log every wrong answer after every mock — by specific topic, not chapter.
    17. Do all spaced repetition revisions due that day. Do not let them accumulate.
    18. Clear backlogs before starting new chapters. The system shows a red banner if you have overdue backlogs.
    19. Regenerate the AI plan after entering new mock data — the plan gets better with each data point.

Using the Heatmap Strategically
Two weeks before the exam, your heatmap should have no red or dark cells. Build a rule: any chapter that is not at least ★3 (yellow) in all sub-topics cannot be considered done.

Biology is 50% of the Paper
360 out of 720 marks come from Biology. The heatmap will immediately show if you are neglecting any Biology chapters. Biology has 38 chapters — more than Physics and Chemistry combined. Small Biology gaps cost more marks than large Physics gaps.

Mock Error Patterns
After 5+ mocks, the error log builds a ranked list of your most repeated mistakes. The AI reads this and prioritises those topics in your daily plan. The same topic appearing in 3+ mocks is a guaranteed backlog item — do not wait for the AI to tell you.

12. Troubleshooting

My data disappeared
Data is stored in localStorage for that specific file URL. This can be lost if you:
    • Opened the file in incognito mode
    • Cleared browser history/cache/site data
    • Moved or renamed the HTML file (the URL changes)
    • Opened the file in a different browser
Prevention: use the same browser, same file location, never incognito.

AI plan not generating
    • Check that your Groq API key is saved in ⚙ Settings
    • Open browser DevTools (F12 → Console) to check for API errors
    • The Groq free tier allows 14,400 requests per day — if you hit the limit, wait until next day
    • Ensure you have an internet connection (the Groq API call requires it)

Calendar sync not working
    • Ensure your Google Calendar is set to PUBLIC
    • Check that your Google Calendar API key is correct in settings
    • The API key must have Google Calendar API enabled in Google Cloud Console
    • If using an organisation Google account, your admin may have restricted public calendar access

Rating modal not appearing
The modal appears only when you tick a chapter from not-done to done (not when un-ticking). If it does not appear, click the ★ stars directly in the chapter list row.

Heatmap showing wrong colours
The heatmap colour is calculated from your topic ratings. If a chapter shows dark even after completion, it means you have not rated its topics yet. Open the rating modal by clicking the ★ stars next to the chapter name.



You have everything you need.
Be consistent. Rate honestly. Clear your backlogs. The 720 will follow.
