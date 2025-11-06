# Sprint 2 Planning - ToDo App (CSC305)

## Sprint Overview

**Sprint Duration**: 2 weeks  
**Sprint Goal**: Enhance user experience with inspirational quotes feature  
**User Stories Planned**: US6  
**Sprint Status**: In Progress

---

## Sprint 2 Backlog

### US6: Inspirational Quotes
**Status**: Sprint Backlog → In Progress  
**Assigned to**: [Your Name]  
**Story Points**: 3  
**Priority**: Low

**Description**: Integrate Zen Quotes API to display inspirational quotes on the dashboard, providing users with motivation while managing their tasks.

**Acceptance Criteria**:
- Dashboard displays a random inspirational quote from Zen Quotes API
- Quote refreshes on page load or user request
- Quote displays author attribution when available
- API errors are handled gracefully with fallback quotes
- Quote display is visually appealing and non-intrusive
- User can manually request a new quote with refresh button
- Quote functionality works across different network conditions

---

## Tasks Breakdown

### Task 1: Zen Quotes API Integration
**Status**: Sprint Backlog  
**Estimated Effort**: 4 hours  
**Parent User Story**: US6  
**Labels**: Task, US6, Sprint 2, [Your Name]

**Description**: Research and implement integration with Zen Quotes API, including error handling and network resilience.

**Subtasks**:
- [ ] Research Zen Quotes API documentation and endpoints
- [ ] Set up API configuration in FlutterFlow
- [ ] Implement API call logic with proper error handling
- [ ] Add retry mechanism for failed requests
- [ ] Test API integration with various network conditions
- [ ] Implement fallback quotes for offline scenarios

**Technical Notes**:
- API Endpoint: https://zenquotes.io/api/random
- No API key required for basic usage
- Rate limit: Check API documentation
- Response format: JSON array with quote and author

---

### Task 2: Quote Display UI
**Status**: Sprint Backlog  
**Estimated Effort**: 3 hours  
**Parent User Story**: US6  
**Labels**: Task, US6, Sprint 2, [Your Name]

**Description**: Design and implement user interface for displaying inspirational quotes on the dashboard.

**Subtasks**:
- [ ] Design quote display component in FlutterFlow
- [ ] Add styling for quote text and author attribution
- [ ] Implement refresh button with appropriate icon
- [ ] Add loading state indicator
- [ ] Ensure responsive design across device sizes
- [ ] Add smooth transitions for quote changes
- [ ] Test UI on multiple devices and screen sizes

**Design Considerations**:
- Quote should be prominently displayed but not overshadow main content
- Use calming colors consistent with app theme
- Author attribution should be clear but secondary to quote
- Refresh button should be intuitive and accessible

---

### Task 3: Testing & FlutterFlow Branch Merge
**Status**: Sprint Backlog  
**Estimated Effort**: 3 hours  
**Parent User Story**: US6  
**Labels**: Task, US6, Sprint 2, [Your Name]

**Description**: Comprehensive testing of quote feature and merge of FlutterFlow branch to main.

**Subtasks**:
- [ ] Write unit tests for API integration logic
- [ ] Perform manual testing of quote display
- [ ] Test error handling scenarios (no network, API down, invalid response)
- [ ] Verify fallback quotes work correctly
- [ ] Test quote refresh functionality
- [ ] Conduct cross-device testing
- [ ] Review code for quality and best practices
- [ ] Merge FlutterFlow branch to main with proper PR documentation
- [ ] Verify deployment to staging environment

**Testing Scenarios**:
1. Normal operation with active network
2. First load with quotes
3. Manual refresh of quotes
4. No network connection (offline mode)
5. API timeout scenarios
6. Malformed API responses
7. Rapid successive refresh requests

---

## Sprint Goals and Success Criteria

### Primary Goals
1. **Complete US6**: Implement fully functional inspirational quotes feature
2. **Quality Delivery**: Ensure robust error handling and user experience
3. **Maintain Velocity**: Complete 3 story points as planned
4. **Zero Technical Debt**: No shortcuts or deferred quality issues

### Success Criteria
- ✅ All acceptance criteria for US6 met
- ✅ All 3 tasks completed and tested
- ✅ Code merged to main branch
- ✅ Feature deployed to staging environment
- ✅ No critical bugs in production
- ✅ Positive stakeholder feedback

---

## Project Board Workflow

### Column States for Sprint 2

1. **Sprint Backlog**: US6 PBI and 3 tasks start here
2. **In Progress**: Cards move here when work begins
3. **Done**: Cards move here when completed and verified

### Expected Card Movement

**Week 1**:
- US6 PBI: Sprint Backlog → In Progress
- Task 1 (API Integration): Sprint Backlog → In Progress → Done
- Task 2 (Quote Display UI): Sprint Backlog → In Progress

**Week 2**:
- Task 2 (Quote Display UI): In Progress → Done
- Task 3 (Testing & Merge): Sprint Backlog → In Progress → Done
- US6 PBI: In Progress → Done

---

## Labels Applied

All cards for Sprint 2 have the following labels:
- **US6**: User story identifier
- **Sprint 2**: Sprint designation
- **[Your Name]**: Assignment label
- **PBI**: For parent user story card
- **Task**: For child task cards

---

## Sprint Risks and Mitigation

### Risk 1: External API Dependency
**Risk**: Zen Quotes API may be unreliable or change without notice  
**Impact**: Medium  
**Mitigation**: Implement fallback quotes stored locally; add comprehensive error handling

### Risk 2: Network Variability
**Risk**: Users may have poor or no network connectivity  
**Impact**: Medium  
**Mitigation**: Implement caching strategy; provide offline fallback quotes

### Risk 3: Scope Creep
**Risk**: Stakeholders may request additional quote features  
**Impact**: Low  
**Mitigation**: Clearly define MVP scope; defer enhancements to future sprints

---

## Definition of Done

A task or user story is considered "Done" when:
- [ ] All acceptance criteria met
- [ ] Code written and follows project standards
- [ ] Code reviewed (self or peer)
- [ ] Unit tests written and passing
- [ ] Manual testing completed
- [ ] Documentation updated
- [ ] No known critical or high-priority bugs
- [ ] Merged to main branch
- [ ] Deployed to staging environment
- [ ] Demonstrated to stakeholders

---

## Daily Standup Notes

### Day 1
- Started Sprint 2 planning
- Created US6 PBI card and 3 task cards
- Set up project board with proper labels
- **Blockers**: None

### Day 2-5
- Working on Task 1: API Integration
- Researching Zen Quotes API
- **Blockers**: [To be updated]

### Day 6-8
- Working on Task 2: Quote Display UI
- **Blockers**: [To be updated]

### Day 9-10
- Working on Task 3: Testing & Merge
- **Blockers**: [To be updated]

---

## Resources and References

- **Zen Quotes API Documentation**: https://zenquotes.io/
- **FlutterFlow Documentation**: https://docs.flutterflow.io/
- **USER_STORIES.md**: Complete user story definitions
- **SPRINT_1.md**: Previous sprint retrospective
- **GITHUB_PROJECT_SETUP.md**: Project board setup guide

---

## Sprint Schedule

**Sprint Start**: [Date]  
**Sprint End**: [Date]  
**Sprint Planning**: Completed  
**Daily Standups**: Daily at [Time]  
**Sprint Review**: [End Date]  
**Sprint Retrospective**: [End Date]

---

## Communication Plan

- **Daily Updates**: Standup notes in this document
- **Blockers**: Escalate immediately via [Communication Channel]
- **Code Reviews**: Via GitHub Pull Requests
- **Sprint Review**: Demo to stakeholders at end of sprint
- **Retrospective**: Team reflection session after sprint review

---

## Next Steps

1. Move US6 PBI from Product Backlog to Sprint Backlog
2. Move Task 1 from Sprint Backlog to In Progress
3. Begin API research and implementation
4. Update project board daily as tasks progress
5. Document any issues or learnings in this file

---

## Notes

- Sprint 2 is focused on quality enhancement rather than core functionality
- This is a lighter sprint (3 points vs 26 in Sprint 1)
- Emphasis on external integration and error handling
- Good opportunity to establish testing best practices
- Screenshots of project board states should be captured for documentation

---

*Sprint 2 in progress. Document updated as sprint progresses.*

---

*Document created: November 2025*
