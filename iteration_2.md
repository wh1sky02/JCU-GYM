# ✅ Actual Iteration-2 Board: JCU Gym Management System

**Start Date:** June 25, 2025  
**End Date:** July 16, 2025  
**Iteration Duration:** 3 weeks

---

## 🔧 Goal

Enhance user engagement and admin visibility by adding booking analytics, automated session reminders, and a virtual gym tour. This iteration focuses on improving usability and system intelligence based on real usage data.

---

## 👥 Team Details

- **Velocity per developer:** 2.5 productive days/week  
- **Team Size:** 4 developers  
- **Total Estimated Workload:** 30 person-days

---

## 📌 User Stories (Iteration 2)

1. **[Booking Statistics](./user_stories/user_story_05_booking_statistics.md)**  
   - **Priority:** Medium  
   - **Estimate:** 4 days  
   - **Description:** Admins can track gym usage trends through a visual dashboard.  
   - **Acceptance Criteria:**  
     - Graphs and summaries of bookings  
     - Filters by session type and date range  
     - Exportable reports (CSV)  
     - Cancellation rate tracking  

2. **[Session Reminders](./user_stories/user_story_06_session_reminders.md)**  
   - **Priority:** Medium  
   - **Estimate:** 3 days  
   - **Description:** Users receive automated reminders ahead of their booked sessions.  
   - **Acceptance Criteria:**  
     - Email or in-app reminders  
     - Admin-defined default timing  
     - User opt-in/opt-out option  
     - Delivery confirmation  

3. **[Virtual Gym Tour](./user_stories/user_story_07_virtual_tour.md)**  
   - **Priority:** Low  
   - **Estimate:** 2 days  
   - **Description:** An online interactive photo tour of the gym for first-time users.  
   - **Acceptance Criteria:**  
     - Key areas shown (e.g., equipment zones, locker rooms)  
     - Works on desktop and mobile  
     - Optional image captions or labels  

---

## 🗓️ Practical 4: Iteration2-week4 Execution & Tracking

### 🎯 Objective
Start development and track progress based on Agile practices from Chapter 4.

### 🛠️ How We Applied It

#### ✅ 1. Split User Stories into Tasks  
Each user story has been broken down into detailed GitHub issues under the `/issues` tab:
- UI components (booking stats, reminders)
- Backend endpoints (FastAPI)
- Notification system (SMTP/Firebase)
- Interactive media for the virtual tour

#### ✅ 2. Monitor Tasks with Labels  
Each task is tracked using GitHub labels:
- `todo`
- `in-progress`
- `done`

#### ✅ 3. Use GitHub Features  
- All issues are assigned to team members with deadlines  
- Status updates are posted in each issue thread  
- GitHub Projects board is used for visual tracking

#### ✅ 4. Commit Daily with Meaningful Messages  
- Team commits follow this format:  
  `feat: add booking stats dashboard`  
  `fix: session reminder delivery bug`  
  `chore: update README and schema`

#### ✅ 5. Use Pull Requests  
- All major features go through pull requests for review  
- Comments and suggestions are made before merging to `main`  
- Ensures code quality and consistency across the team

---

## 📋 Sprint Backlog Status

### 🟡 In Progress
- Booking Statistics  
- Session Reminders  

### ✅ Completed
- Virtual Gym Tour (to be updated during sprint review)

---

## 📉 Burndown Chart – Iteration 2

| Week     | Estimated Days Remaining |
|----------|--------------------------|
| Week 4   | 4 days                   |
| Week 3   | 10 days                  |
| Week 2   | 7 days                   |
| Week 1   | 0 days                   |

**Actual Velocity:** 2.4 person-days/week (calculated post-sprint)

---

## 📦 Key Deliverables

- [ ] Admin dashboard with booking analytics  
- [ ] Automated session reminders  
- [ ] Interactive virtual gym tour  
- [ ] Improved mobile experience  
- [ ] Backend performance improvements  
- [ ] Optional personalization features

---

## 🛠️ Technical Stack

- **Frontend:** React.js  
- **Backend:** FastAPI (Python)  
- **Database:** PostgreSQL  
- **Analytics:** Chart.js / Plotly  
- **Notifications:** SMTP / Firebase  
- **Authentication:** JWT
