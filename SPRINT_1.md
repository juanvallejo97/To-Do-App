# Sprint 1 Retrospective - ToDo App (CSC305)

## Sprint Overview

**Sprint Duration**: 2 weeks  
**Sprint Goal**: Implement core functionality for user authentication, profile management, and task management  
**User Stories Completed**: US1, US2, US3, US4, US5

---

## Completed User Stories

### US1: Account Creation ✅
**Status**: Done  
**Assigned to**: [Your Name]  
**Story Points**: 5

**Completed Tasks**:
- Task: Design registration form UI in FlutterFlow
- Task: Implement backend validation logic
- Task: Add secure password storage with encryption
- Task: Test registration flow with various input scenarios

**Outcome**: Users can successfully create accounts with email and password. All validation rules are working as expected.

---

### US2: Login/Create Page ✅
**Status**: Done  
**Assigned to**: [Your Name]  
**Story Points**: 3

**Completed Tasks**:
- Task: Create login page UI with FlutterFlow
- Task: Implement authentication logic
- Task: Add session management
- Task: Test login flow and error handling

**Outcome**: Login functionality is fully operational. Users can authenticate and sessions are properly managed.

---

### US3: User Profile Editing ✅
**Status**: Done  
**Assigned to**: [Your Name]  
**Story Points**: 5

**Completed Tasks**:
- Task: Design profile editing interface
- Task: Implement update functionality for user data
- Task: Add validation for profile changes
- Task: Test profile update scenarios

**Outcome**: Users can successfully edit their profile information with proper validation and confirmation.

---

### US4: Dashboard ✅
**Status**: Done  
**Assigned to**: [Your Name]  
**Story Points**: 8

**Completed Tasks**:
- Task: Design dashboard layout in FlutterFlow
- Task: Implement CRUD operations for to-do items
- Task: Add filtering and sorting functionality
- Task: Integrate real-time updates
- Task: Test dashboard performance and functionality

**Outcome**: Dashboard provides comprehensive task management with all CRUD operations working smoothly. Performance is acceptable with multiple items.

---

### US5: Checkout Page ✅
**Status**: Done  
**Assigned to**: [Your Name]  
**Story Points**: 5

**Completed Tasks**:
- Task: Create checkout/review page UI
- Task: Implement batch update confirmation logic
- Task: Add navigation flow
- Task: Test checkout process

**Outcome**: Checkout page allows users to review and confirm task updates before finalizing changes.

---

## Sprint Metrics

- **Total Story Points Committed**: 26
- **Total Story Points Completed**: 26
- **Velocity**: 26 points/sprint
- **Sprint Completion Rate**: 100%

### Burndown Chart Summary
- Sprint started with 26 points
- Steady progress throughout sprint
- All points completed by end of sprint
- No carryover items

---

## What Went Well

1. **Strong Team Collaboration**: Clear communication throughout the sprint helped identify and resolve issues quickly
2. **Effective Planning**: Breaking user stories into smaller tasks made progress tracking easier
3. **FlutterFlow Efficiency**: Using FlutterFlow significantly accelerated UI development
4. **Complete Core Features**: All essential functionality for the app is now in place
5. **Quality Delivery**: All acceptance criteria met for completed user stories

---

## What Could Be Improved

1. **Testing Coverage**: Could benefit from more comprehensive automated tests
2. **Code Documentation**: Some backend logic needs better inline documentation
3. **Time Estimation**: Dashboard (US4) took longer than initially estimated
4. **API Design**: Backend API could be optimized for fewer round-trips
5. **Error Handling**: Some edge cases in error handling could be more robust

---

## Action Items for Next Sprint

1. **Improve Testing**: Add unit and integration tests for critical paths
2. **Documentation**: Add inline code comments for complex logic
3. **Performance Optimization**: Review and optimize API calls
4. **Enhanced Error Handling**: Implement comprehensive error handling for all user flows
5. **Code Review Process**: Establish peer review before merging to main branch

---

## Blockers and Resolutions

### Blocker 1: FlutterFlow Backend Integration
- **Issue**: Initial difficulty connecting FlutterFlow frontend to custom backend
- **Resolution**: Reviewed documentation and implemented proper API endpoints with CORS configuration
- **Impact**: Delayed US4 by 1 day

### Blocker 2: Session Management
- **Issue**: Session tokens expiring inconsistently
- **Resolution**: Implemented refresh token mechanism
- **Impact**: Minor delay in US2, resolved within sprint

---

## Technical Debt Identified

1. **Database Optimization**: Current schema could be normalized for better performance
2. **Security Enhancements**: Implement rate limiting for API endpoints
3. **Responsive Design**: Dashboard needs optimization for tablet/desktop views
4. **Offline Support**: Consider implementing offline-first architecture
5. **Code Refactoring**: Some components have duplicated logic that should be abstracted

---

## Demo Highlights

During sprint review, the following features were demonstrated:
- Complete user registration and authentication flow
- Profile management with real-time updates
- Full task CRUD operations on dashboard
- Checkout/review workflow for task updates

**Stakeholder Feedback**: Positive reception overall. Feature requests noted for future sprints.

---

## Sprint 2 Preview

**Focus**: Enhancement features  
**Planned User Stories**: US6 (Inspirational Quotes)  
**Goals**: 
- Integrate Zen Quotes API
- Add motivational elements to user experience
- Implement error handling for external API dependency
- Maintain code quality and testing standards

---

## Team Notes

- All Sprint 1 PBI cards and tasks have been moved to **Done** column on project board
- Labels properly applied: US1-US5, Sprint 1, [Your Name], PBI, Task
- GitHub project board reflects accurate sprint completion status
- All code merged to main branch and deployed to staging environment

---

## Retrospective Participants

- [Your Name] - Developer
- Project Supervisor - Product Owner
- Course Instructor - Stakeholder

**Meeting Date**: [End of Sprint 1]  
**Next Retrospective**: [End of Sprint 2]

---

*Sprint 1 completed successfully with all objectives met. Ready to proceed to Sprint 2.*

---

*Document created: November 2025*
