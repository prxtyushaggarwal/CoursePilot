# CoursePilot · Smart Academic Performance & Timetable Attendance Hub
> **Lovely Professional University (LPU) · Department of Full Stack Application Development**  
> **Course:** INT335 · Design Thinking · Session 2026–27 (Section K4P26NY)  
> **Component:** Continuous Assessment (CA2) Comprehensive Project & Working Showcase  

---

## 🚀 Live Demo & Quick Launch

- **Live URL (Local Server):** `http://localhost:8000/index.html`
- **Or simply open:** `index.html` in any modern web browser (Chrome, Edge, Firefox, Safari). Zero dependencies, zero build steps needed!

---

## 📌 Project Overview

**CoursePilot** is an intelligent academic management and adaptive study planning web application designed specifically around the Lovely Professional University student workflow. It solves academic planning paralysis by integrating:
1. **Daily Timetable & Attendance Roll Call:** Synchronized directly with LPU Class Schedule **Section K4P26NY**.
2. **Attendance Calculation & 75% Debarment Guard:** Supports **Present (✓)**, **Absent (✗)**, **Duty Leave (DL)**, and **Class Cancelled** options with real-time percentage recalculation and margin buffers.
3. **Continuous Assessment (CA) Ledger:** Implements the university's official **Best 2-of-3 CA rule** scaled to 30 marks.
4. **Dedicated Examination Hub:** Independent tracking for **Mid-Term Exams (MTT - 30 marks)** and predictive target calculators for **End-Term Exams (ETT - 100 marks)**.
5. **Authentic 6-Unit Syllabus Tracker:** Pre-loaded with official syllabi for all 6 active courses.
6. **AI Copilot & Resource Discovery Engine:** Instant search for curated YouTube playlists (Gate Smashers, Abdul Bari, Tikle's Academy, GP Sir, CodeWithHarry), GitHub student notes, and GeeksforGeeks guides.
7. **INT335 Design Thinking Showcase:** Integrated 12-slide evaluator presentation deck and the full 22-part project report.

---

## 📚 Enrolled Courses & Authentic Syllabi (Section K4P26NY)

| Course Code | Course Title | Credits | Description & Syllabus Scope |
| :--- | :--- | :---: | :--- |
| **CSE111** | **Orientation to Computing** | 3 | Computer hardware, memories, OS architecture, Linux directory hierarchy & bash commands, cohorts, Git/GitHub developer branding. |
| **CSE326** | **Internet Programming** | 4 | HTML5 fundamentals, complex tables & forms, CSS3 Box Model & Flexbox, JavaScript DOM manipulation, event handling & GitHub Pages. |
| **INT108** | **Python Programming** | 3 | Environment setup, loops & branching, strings/lists/tuples/dicts, functions & recursion, OOP (classes & inheritance), and file handling/RegEx. |
| **INT335** | **Design Thinking** | 2 | Empathize (AEIOU & personas), Define (POV & HMW), Ideate (Crazy 8s & weighted screening matrix), Paper/Digital MVP, and silent testing. |
| **MEC136** | **Engineering Drawing with AutoCAD** | 3 | Scales & lettering, orthographic projections of points/lines/planes, first & third angle systems, sectional views, isometric views, and 3D modeling. |
| **MTH165** | **Mathematics for Engineers** | 4 | Linear algebra (rank, eigenvalues & Cayley-Hamilton), differential/integral calculus, mean value theorems, partial derivatives, multiple integrals, and Fourier series. |

---

## 📅 Timetable Schedule Matrix (Section K4P26NY)

| Day | Period 1 | Period 2 | Period 3 | Period 4 | Period 5 | Period 6 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Monday** | `10:10-11:00` MEC136 (25-101A) | `11:00-11:50` MEC136 (25-101A) | `12:40-13:30` MTH165 (26-407) | — | — | — |
| **Tuesday** | `10:10-11:00` CSE326 (26-102) | `11:00-11:50` CSE326 (26-102) | `11:50-12:40` MTH165 (25-702) | — | — | — |
| **Wednesday** | `10:10-11:00` INT108 (27-406) | `11:00-11:50` INT108 (27-406) | `11:50-12:40` CSE111 (27-406) | — | — | — |
| **Thursday** | `10:10-11:00` CSE326 (25-505) | `11:00-11:50` INT335 (25-505) | `11:50-12:40` INT108 (25-505) | `12:40-13:30` INT108 (25-505) | `13:30-14:20` MTH165 (25-505) | `16:00-16:50` CSE111 (38-904) |
| **Friday** | `10:10-11:00` INT335 (25-101A) | `11:00-11:50` CSE111 (25-101A) | `11:50-12:40` MTH165 (25-101A) | `12:40-13:30` MEC136 (27-404X)| `14:20-15:10` INT108 (26-109) | `15:10-16:00` INT108 (26-109) |
| **Saturday** | *No Classes (Weekend)* | — | — | — | — | — |
| **Sunday** | *No Classes (Weekend)* | — | — | — | — | — |

---

## 🧮 Mathematical Models & Core Algorithms

### 1. Attendance Percentage & Policy Engine
$$\text{Attendance \%} = \frac{\text{Present} + \text{Duty Leave (DL)}}{\text{Total Held (excluding Cancelled)}} \times 100$$
- **Duty Leave (DL):** Counted as Present (technically 100%).
- **Class Cancelled:** When a faculty member does not take class, it is excluded from total held sessions so students are not penalized.
- **75% Mandatory Criteria:** When attendance drops below 75%, per-subject danger badges and overall campus alerts trigger immediately.

### 2. Adaptive Study Priority Engine
$$P_i = 0.5 \times W_i + 0.3 \times E_i + 0.2 \times S_i$$
Where:
- $W_i = 100 - \text{Quiz/Self-Assessment Score} \in [0, 100]$ (Weakness)
- $E_i = \max\left(0, 100 - \frac{\text{Days Until Exam}}{30} \times 100\right)$ (Urgency)
- $S_i = 100 \text{ if Pending, } 20 \text{ if Completed}$ (Syllabus status)

---

## 📂 Repository File Structure



## 🛠️ Step-by-Step Instructions to Push to GitHub

Open your terminal or PowerShell in this directory:

```bash



