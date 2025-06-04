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
| Week 3   | 10 days                  |
| Week 2   | 7 days                   |
| Week 1   | 3 days                   |
| Week 0   | 0 days                   |

**Actual Velocity:** To be calculated post-sprint

---

## 📦 Key Deliverables

- [x] Fully functional user registration system  
- [x] Admin panel for user control  
- [ ] Gym session booking flow  
- [ ] Booking cancellation feature  
- [ ] Backend APIs + database setup  
- [ ] Clean user/admin interface

---

## 🛠️ Technical Stack

- **Frontend:** React.js  
- **Backend:** FastAPI (Python)  
- **Database:** PostgreSQL  
- **Authentication:** JWT
