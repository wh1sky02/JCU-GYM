### ✅ Iteration 1: Done and Dusted

**Finished on:** June 24, 2025  
**Total Work Done:** 30 person-days  
**Team Velocity:** Around 2.5 productive days per developer each week  

---

#### 🗂️ What We’ve Checked Off

- [x] Built and tested all user stories  
- [x] Completed everything in the sprint backlog  
- [x] Created burndown and velocity charts  
- [x] Functional prototype up and running  
- [x] GitHub board and workflows are in place  

---

### 📝 Wrap-up Notes

We hit our targets and got the core features working smoothly.  
No major blockers this sprint, and progress stayed steady throughout.  
Some improvements like polishing the interface and UX tweaks will carry over into Iteration 2.

---
# ✅ Actual Iteration-1 Board: JCU Gym Management System

**Start Date:** June 3, 2025  
**End Date:** June 24, 2025  
**Iteration Duration:** 3 weeks

---

## 🔧 Goal

Develop the foundational features of the JCU Gym Management System, including user registration, gym session booking, and admin controls. These features will allow a functional prototype with secure user access and booking flow.

---

## 👥 Team Details

- **Velocity per developer:** 2.5 productive days/week  
- **Team Size:** 4 developers  
- **Total Estimated Workload:** 30 person-days

---

## 📌 User Stories (Iteration 1)

1. **[User Registration](./user_stories/user_story_01_registration.md)**  
   - **Priority:** High  
   - **Estimate:** 3 days  
   - **Description:** Allow new users to sign up securely with email and password.  
   - **Acceptance Criteria:**  
     - Registration form with name, JCU email, and password  
     - Password validation and hashing  
     - Confirmation on successful signup  
     - Store user data securely in the database  

2. **[Session Booking](./user_stories/user_story_02_session_booking.md)**  
   - **Priority:** High  
   - **Estimate:** 4 days  
   - **Description:** Users can view and book available gym sessions.  
   - **Acceptance Criteria:**  
     - Display available sessions (date, time, slots)  
     - Booking form linked to user  
     - Prevent double-booking  
     - Securely store booking data  

3. **[Admin User Management](./user_stories/user_story_03_admin_management.md)**  
   - **Priority:** High  
   - **Estimate:** 3 days  
   - **Description:** Admin dashboard for managing users.  
   - **Acceptance Criteria:**  
     - View all registered users  
     - Approve or reject users  
     - Secure admin-only access  

4. **[Manage Bookings](./user_stories/user_story_04_manage_bookings.md)**  
   - **Priority:** Medium  
   - **Estimate:** 3 days  
   - **Description:** Let users view and cancel upcoming gym bookings.  
   - **Acceptance Criteria:**  
     - Display all upcoming bookings  
     - Allow cancellation for non-same-day sessions  
     - Update session availability in real-time  
     - Send cancellation confirmation  

---

## 📋 Sprint Backlog Status

### 🟡 In Progress
- Session Booking  
- Manage Bookings  

### ✅ Completed
- User Registration  
- Admin User Management  

---

## 📉 Burndown Chart – Iteration 1

| Week     | Estimated Days Remaining |
|----------|--------------------------|
| Week 4   | 8 days                   |
| Week 3   | 10 days                  |
| Week 2   | 7 days                   |
| Week 1   | 3 days                   |
| Week 0   | 0 days                   |

**Actual Velocity:** Will be calculated at the end of the iteration.

---

## 📦 Key Deliverables

- [x] Fully functional user registration system  
- [x] Admin panel for user control  
- [ ] Gym session booking flow  
- [ ] Booking cancellation feature  
- [ ] Backend APIs + database setup  
- [ ] Clean user/admin interface  
- [ ] GitHub project board tracking  
- [ ] Pull request and issue workflows established

---

## 🛠️ Technical Stack

- **Frontend:** React.js  
- **Backend:** FastAPI (Python)  
- **Database:** PostgreSQL  
- **Authentication:** JWT  
- **Tracking:** GitHub Issues, Labels, Pull Requests, Projects

---

## 📌 User Stories (Iteration 1)

### 1. User Registration (3 days)
- **Priority:** High
- **Estimate:** 3 days
- **Description:** Allow new users to sign up securely with email and password.
- **Acceptance Criteria:**
  - Registration form with name, JCU email, and password
  - Password validation and hashing
  - Confirmation on successful signup
  - Store user data securely in the database

#### Tasks:
- **Task 1:** Design and implement registration form (TODO)
- **Task 2:** Implement email and password validation (TODO)
- **Task 3:** Implement password hashing for security (TODO)
- **Task 4:** Implement confirmation on successful signup (TODO)
- **Task 5:** Store user data securely in the database (TODO)
- **Task 6:** Test registration flow (TODO)

---

### 2. Session Booking (4 days)
- **Priority:** High
- **Estimate:** 4 days
- **Description:** Users can view and book available gym sessions.
- **Acceptance Criteria:**
  - Display available sessions (date, time, slots)
  - Booking form linked to user
  - Prevent double-booking
  - Securely store booking data

#### Tasks:
- **Task 1:** Display available sessions on the UI (TODO)
- **Task 2:** Implement session booking form linked to user (TODO)
- **Task 3:** Implement session availability check to prevent double-booking (TODO)
- **Task 4:** Store booking data securely in the database (TODO)
- **Task 5:** Test booking functionality (TODO)

---

### 3. Admin User Management (3 days)
- **Priority:** High
- **Estimate:** 3 days
- **Description:** Admin dashboard for managing users.
- **Acceptance Criteria:**
  - View all registered users
  - Approve or reject users
  - Secure admin-only access

#### Tasks:
- **Task 1:** Design and implement admin dashboard (TODO)
- **Task 2:** Implement user approval/rejection functionality (TODO)
- **Task 3:** Implement secure admin-only access to the dashboard (TODO)
- **Task 4:** Test admin dashboard functionality (TODO)

---

### 4. Manage Bookings (3 days)
- **Priority:** Medium
- **Estimate:** 3 days
- **Description:** Let users view and cancel upcoming gym bookings.
- **Acceptance Criteria:**
  - Display all upcoming bookings
  - Allow cancellation for non-same-day sessions
  - Update session availability in real-time
  - Send cancellation confirmation

#### Tasks:
- **Task 1:** Display user's upcoming bookings on the UI (TODO)
- **Task 2:** Implement cancellation functionality for non-same-day sessions (TODO)
- **Task 3:** Implement real-time session availability update (TODO)
- **Task 4:** Send cancellation confirmation to users (TODO)
- **Task 5:** Test booking management and cancellation functionality (TODO)
