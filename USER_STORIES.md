# User Stories for ToDo App (CSC305)

This document outlines the user stories for the ToDo App project, organized by sprint and feature area.

---

## US1: Account Creation

**As a** new user  
**I want to** create an account with my email and password  
**So that** I can securely access my personalized to-do list

### Acceptance Criteria
- User can register with a valid email address
- Password must meet minimum security requirements (8+ characters, includes numbers and special characters)
- System validates email format before account creation
- User receives confirmation message upon successful registration
- Duplicate email addresses are rejected with appropriate error message
- Account data is securely stored in the backend

### Priority
High

### Story Points
5

---

## US2: Login/Create Page

**As a** registered user  
**I want to** log in with my credentials  
**So that** I can access my personal to-do list and account information

### Acceptance Criteria
- User can enter email and password on login page
- System validates credentials against stored account data
- Successful login redirects user to dashboard
- Failed login displays clear error message
- "Forgot password" option is available
- Session is maintained until user logs out or timeout occurs
- Login page has link to account creation for new users

### Priority
High

### Story Points
3

---

## US3: User Profile Editing

**As a** registered user  
**I want to** edit my profile information  
**So that** I can keep my account details current and personalized

### Acceptance Criteria
- User can access profile editing page from dashboard
- User can update display name, email, and password
- Email changes require re-validation
- Password changes require current password confirmation
- Changes are saved securely to backend
- User receives confirmation message after successful update
- User can cancel changes without saving

### Priority
Medium

### Story Points
5

---

## US4: Dashboard

**As a** registered user  
**I want to** view and manage my to-do items on a dashboard  
**So that** I can efficiently organize and track my tasks

### Acceptance Criteria
- Dashboard displays all user's to-do items
- User can add new to-do items with title and description
- User can mark items as complete/incomplete
- User can edit existing to-do items
- User can delete to-do items with confirmation
- Items are organized by status (pending/completed)
- Dashboard loads quickly and displays real-time updates
- User can filter/sort items by date, priority, or status

### Priority
High

### Story Points
8

---

## US5: Checkout Page

**As a** user  
**I want to** review and confirm my task completion  
**So that** I can ensure accuracy before finalizing my to-do list updates

### Acceptance Criteria
- User can access checkout/review page from dashboard
- Page displays summary of pending task updates
- User can review changes before confirming
- User can confirm or cancel batch updates
- Confirmed changes are saved to backend
- User receives confirmation message
- User is redirected to dashboard after completion

### Priority
Medium

### Story Points
5

---

## US6: Inspirational Quotes

**As a** user  
**I want to** see inspirational quotes on my dashboard  
**So that** I can stay motivated while managing my tasks

### Acceptance Criteria
- Dashboard displays a random inspirational quote from Zen Quotes API
- Quote refreshes on page load or user request
- Quote displays author attribution when available
- API errors are handled gracefully with fallback quotes
- Quote display is visually appealing and non-intrusive
- User can manually request a new quote with refresh button
- Quote functionality works across different network conditions

### Priority
Low

### Story Points
3

### Technical Notes
- Uses Zen Quotes API (https://zenquotes.io/)
- Requires API integration and error handling
- Should implement caching strategy for offline support

---

## Sprint Allocation

- **Sprint 1**: US1, US2, US3, US4, US5 (Core functionality)
- **Sprint 2**: US6 (Enhancement features)

---

## Notes

- Story points estimated using Fibonacci scale (1, 2, 3, 5, 8, 13)
- Priorities: High (critical functionality), Medium (important features), Low (nice-to-have enhancements)
- All user stories follow the format: "As a [user type], I want to [action], so that [benefit]"

---

*Last updated: November 2025*
