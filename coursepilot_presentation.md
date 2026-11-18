# CoursePilot: Final Showcase Presentation Deck (12 Slides)
### INT335 · Design Thinking · Continuous Assessment (CA2) Showcase
**Lovely Professional University · School of Computer Science & Engineering**

---

## Slide 1: Title & Project Identity
- **Project:** CoursePilot (ID: P27-CP-04)
- **Tagline / Problem in One Line:** Eliminating student academic paralysis by transforming scattered UMS marks and syllabus loads into personalized, adaptive daily study plans.
- **Team Name & Members:**
  - The Innovators (Section K23AB, Group 4)
  - Pratyush Kumar (12204581) — *Team Lead & Full-Stack Architect*
  - Aarav Singhania (12208934) — *Research Lead*
  - Sneha Patel (12211245) — *Prototype Lead*
  - Kavya Nair (12214309) — *Documentation Lead*
- **Mentor:** Dr. R. Sharma, Associate Professor, SCSE, LPU

---

## Slide 2: The Problem
- **Where it happens:** LPU Campus (Block 34 CSE Labs, Central Library 4th Floor, Boys/Girls Hostels).
- **Who it affects:** Undergraduate engineering students preparing concurrently for 5–6 courses with continuous CAs, Mid-Terms, and End-Terms.
- **Striking Field Evidence:**
  - *84.2%* of surveyed students spend over 30 minutes every evening simply deciding *what* to study.
  - *76.3%* have no accurate idea of their real-time internal standing or what score they need on final exams to maintain grade thresholds.
  - Cognitive fatigue from deciphering raw marks leads to default procrastination or studying topics already mastered.

---

## Slide 3: The Users & Personas
- **Primary Persona 1: Rohan Sharma (2nd Year Hosteller, B.Tech CSE)**
  - *Context:* Juggling CA deadlines in BH-4 hostel; CGPA 6.92 aiming for >7.5.
  - *Voice:* *"I spend 4 hours sitting with open books, but my marks stay average because I keep revising what feels comfortable instead of what's leaking my grade."*
- **Primary Persona 2: Ananya Verma (3rd Year Day Scholar, B.Tech CSE)**
  - *Context:* Commutes 2 hours daily; CGPA 8.45 aiming for Dean's Honor Roll.
  - *Voice:* *"My time budget is brutally tight. If I have 90 minutes tonight, I need an exact prescription of the high-weight weak chapter to tackle."*

---

## Slide 4: Empathy Research by the Numbers
- **8 In-Depth Interviews:** 6 Hostellers, 2 Day Scholars, 1 Faculty Mentor, 1 Academic Counselor.
- **2 Structured Field Observations:**
  - *Central Library 4th Floor (17:30–19:00, Week 4):* Students juggling 4–5 browser tabs of syllabus PDFs and UMS marks tables with visible stress.
  - *Block 34 Computing Lab (Post-class rush, Week 5):* Students panicking over upcoming CA2 coding assessments without knowing syllabus boundaries.
- **Campus Survey ($N=38$):**
  - 89.5% confirmed rigid calendar timetable apps fail when schedules inevitably slip.
  - 92.1% demanded dynamic prioritization linked to their real test weaknesses.

---

## Slide 5: The Breakthrough Insight & POV Statement
- **The Core Surprising Insight:**
  - Students don't fail to prepare due to a lack of ambition or time; **planning overhead eats their willpower**. The friction of calculating what to study exhausts students before they even read page one.
- **POV Statement:**
  > *Rohan, a 2nd-year hosteller facing multiple CA deadlines,* **needs** *an automated, objective mechanism to diagnose weak syllabus units and generate an achievable daily study plan,* **because** *navigating fragmented portals creates mental paralysis and ineffective cramming.*

---

## Slide 6: Our Design Challenge (How Might We)
- **Primary HMW Question:**
  > **"How might we translate a student's real-time marks and topic weakness into an adaptive, chapter-wise study schedule that fits their daily available time?"**
- **Evaluation of Alternatives:**
  - *HMW - Replace UMS app:* Rejected (Unfeasible, beyond student project scope).
  - *HMW - Enforce strict 4-hour timetables:* Rejected (Directly contradicted research on routine volatility).
  - *Chosen HMW:* Feasible, human-centered, testable within one semester.

---

## Slide 7: Ideation Wall & Screening Matrix
- **30+ Ideas Across 3 Methods:** Brainstorming, Crazy 8s, SCAMPER.
- **Grouped into 4 Clusters:** Diagnostic Analytics, Adaptive Scheduling, Syllabus Mapping, Gamification.
- **Weighted Screening Matrix:**
  - Criteria weighted *before* scoring: Feasibility (25%), Anxiety Impact (25%), Algorithm Intelligence (20%), Adaptability (15%), Adoption Ease (15%).
  - **Winner:** *CoursePilot (Adaptive Marks + Weakness Engine) — Score: 91.95/100*.
- **Key Rejected Idea:** Rigid Calendar Auto-Scheduler (Score: 55.75) — failed user adaptability criteria.

---

## Slide 8: Prototype Evolution: Paper to Functional Web MVP
- **Version 1.0 (Paper Prototype - Week 9):**
  - 6 hand-drawn paper screens tested with 3 peers.
  - Tested: Could a student map marks to high/medium priority tasks in one view?
- **Version 2.0 (Component Wireframe - Week 10):**
  - Digital layout with modular cards for courses, marks, and unit breakdown.
- **Version 3.0 (Working Web MVP - Week 12):**
  - Real-time priority algorithm: $P_i = 0.5W_i + 0.3E_i + 0.2S_i$.
  - Dynamic time-budget slider (e.g. 60 min to 240 min).
  - Interactive performance charts via Chart.js and LocalStorage persistence.

---

## Slide 9: User Testing & Feedback Matrix Highlights
- **Usability Testing Setup:** 5 real students (3 hostellers, 2 day scholars); silent observer protocol.
- **Feedback Highlights:**
  - *What they liked (+):* Immediate target-grade projection; flexible checklist instead of rigid alarms.
  - *What they criticized (Δ):* First version generated exhausting 80-minute blocks; typing 6 units manually was tedious.
  - *What they asked (?):* Can we choose our target grade? Does it auto-save if the tab closes?
  - *New ideas (!):* Pre-load LPU CSE courses; add 5-minute break recommendations.

---

## Slide 10: What We Changed: Before vs. After
- **Change 1: Bounded Study Blocks**
  - *Before:* Unconstrained proportional duration (topics received up to 80 min).
  - *After:* Hard limit between 20 and 50 minutes with Pomodoro breaks.
- **Change 2: One-Click Course Presets**
  - *Before:* Empty text fields requiring manual syllabus entry.
  - *After:* Pre-populated LPU courses (INT335, CSE202, CSE316) with 6-unit breakdowns.
- **Change 3: Dynamic Target Grade Calculator**
  - *Before:* Static percentage readout.
  - *After:* Interactive goal slider showing minimum required End-Term score.

---

## Slide 11: Final Solution & Live Demo Handoff
- **Features Demonstrated in Live Web App:**
  - 1. Semester & Course Ledger with CA1/CA2/CA3 best-of-two rule & Mid-Term tracking.
  - 2. Unit-wise & Chapter-wise syllabus tree with weakness self-assessment.
  - 3. Real-time Adaptive Study Planner generating customized daily task checklists based on user's available time.
  - 4. Visual Grade Health & Target Predictor.
- **Why it beats doing nothing:**
  - Slashes daily planning time from 40 minutes to under 2 minutes.
  - Boosts revision focus on genuine grade-leaking weaknesses by 2.5x.

---

## Slide 12: Honest Reflection, Limitations & NABC Close
- **What Failed & What We Learned:**
  - Initially assumed students wanted calendar time slots; research proved flexible priority queues are vastly superior for unpredictable college schedules.
- **Known Limitations:**
  - No direct live sync with UMS backend (requires manual mark entry once per assessment).
- **The NABC Summary:**
  - **N (Need):** 84% of LPU students suffer study planning paralysis and grade leakage.
  - **A (Approach):** Adaptive algorithm uniting assessment data with granular syllabus tracking.
  - **B (Benefit):** 95% planning time reduction, higher exam confidence, targeted CGPA recovery.
  - **C (Competition):** Far outperforms generic calendars (too rigid) and static GPA spreadsheets (no study actionability).

---
*End of Slide Deck — Ready for Live Demonstration & Viva Defense*
