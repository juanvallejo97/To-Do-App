# GitHub Project Setup Guide - ToDo App (CSC305)

This document provides detailed instructions for setting up and managing the GitHub Project Board for the ToDo App, following agile sprint-based methodology.

---

## Table of Contents

1. [Project Board Structure](#project-board-structure)
2. [Labels Setup](#labels-setup)
3. [Creating PBI Cards](#creating-pbi-cards)
4. [Creating Task Cards](#creating-task-cards)
5. [Workflow Management](#workflow-management)
6. [Sprint 1 Setup (Retrospective)](#sprint-1-setup-retrospective)
7. [Sprint 2 Setup (Current)](#sprint-2-setup-current)
8. [Best Practices](#best-practices)
9. [Screenshots and Evidence](#screenshots-and-evidence)
10. [Troubleshooting](#troubleshooting)

---

## Project Board Structure

### Creating the Project Board

1. Navigate to your repository: `juanvallejo97/To-Do-App`
2. Click on the **Projects** tab
3. Click **New Project**
4. Select **Board** view
5. Name it: "ToDo App - CSC305"
6. Add description: "Agile sprint-based project management for CSC305 ToDo App"

### Column Setup

Create four columns in this exact order:

1. **Product Backlog**
   - Purpose: All user stories not yet scheduled
   - Initial state for new PBIs

2. **Sprint Backlog**
   - Purpose: User stories and tasks planned for current sprint
   - Items move here during sprint planning

3. **In Progress**
   - Purpose: Work actively being done
   - Items move here when development starts

4. **Done**
   - Purpose: Completed and verified work
   - Items move here when all acceptance criteria met

---

## Labels Setup

### Creating Labels

Navigate to: Repository → Issues → Labels → New Label

Create the following labels with suggested colors:

#### User Story Labels
- **US1** - Color: `#0075ca` (Blue) - Description: "User Story 1: Account Creation"
- **US2** - Color: `#0075ca` (Blue) - Description: "User Story 2: Login/Create Page"
- **US3** - Color: `#0075ca` (Blue) - Description: "User Story 3: User Profile Editing"
- **US4** - Color: `#0075ca` (Blue) - Description: "User Story 4: Dashboard"
- **US5** - Color: `#0075ca` (Blue) - Description: "User Story 5: Checkout Page"
- **US6** - Color: `#0075ca` (Blue) - Description: "User Story 6: Inspirational Quotes"

#### Sprint Labels
- **Sprint 1** - Color: `#d4c5f9` (Purple) - Description: "Sprint 1 - Core Features"
- **Sprint 2** - Color: `#d4c5f9` (Purple) - Description: "Sprint 2 - Enhancements"

#### Type Labels
- **PBI** - Color: `#fbca04` (Yellow) - Description: "Product Backlog Item (User Story)"
- **Task** - Color: `#c5def5` (Light Blue) - Description: "Task (Child of PBI)"

#### Assignment Label
- **[Your Name]** - Color: `#7057ff` (Purple) - Description: "Assigned to [Your Name]"
  - Replace `[Your Name]` with your actual name (e.g., "Juan Vallejo")

---

## Creating PBI Cards

PBI (Product Backlog Item) cards represent user stories. Create one issue for each user story.

### PBI Card Template

#### Title Format
```
To-Do-App #[NUMBER] - US[X]: [User Story Title]
```

Example: `To-Do-App #1 - US1: Account Creation`

#### Description Template

```markdown
## User Story

**As a** [user type]  
**I want to** [action]  
**So that** [benefit]

## Acceptance Criteria

- [ ] [Criterion 1]
- [ ] [Criterion 2]
- [ ] [Criterion 3]
- [ ] [Additional criteria...]

## Story Points

[Number of points]

## Priority

[High/Medium/Low]

## Related User Story

See USER_STORIES.md - US[X] for complete details

## Tasks

This user story includes the following tasks:

- [ ] Task: [Task 1 Name] (Issue #[NUMBER])
- [ ] Task: [Task 2 Name] (Issue #[NUMBER])
- [ ] Task: [Task 3 Name] (Issue #[NUMBER])

## Notes

[Any additional technical notes, dependencies, or considerations]
```

### Creating US6 PBI Example

**Step by step:**

1. Go to: Repository → Issues → New Issue
2. **Title**: `To-Do-App #6 - US6: Inspirational Quotes`
3. **Description**: (Copy from USER_STORIES.md US6 section, following template above)
4. **Labels**: Add `US6`, `Sprint 2`, `[Your Name]`, `PBI`
5. **Project**: Assign to "ToDo App - CSC305" project
6. **Column**: Place in "Product Backlog" initially
7. Click **Submit new issue**

**Full Example Description:**

```markdown
## User Story

**As a** user  
**I want to** see inspirational quotes on my dashboard  
**So that** I can stay motivated while managing my tasks

## Acceptance Criteria

- [ ] Dashboard displays a random inspirational quote from Zen Quotes API
- [ ] Quote refreshes on page load or user request
- [ ] Quote displays author attribution when available
- [ ] API errors are handled gracefully with fallback quotes
- [ ] Quote display is visually appealing and non-intrusive
- [ ] User can manually request a new quote with refresh button
- [ ] Quote functionality works across different network conditions

## Story Points

3

## Priority

Low

## Related User Story

See USER_STORIES.md - US6 for complete details

## Tasks

This user story includes the following tasks:

- [ ] Task: Zen Quotes API Integration (Issue #7)
- [ ] Task: Quote Display UI (Issue #8)
- [ ] Task: Testing & FlutterFlow Branch Merge (Issue #9)

## Technical Notes

- Uses Zen Quotes API (https://zenquotes.io/)
- Requires API integration and error handling
- Should implement caching strategy for offline support

## Sprint Allocation

Sprint 2
```

---

## Creating Task Cards

Task cards are child issues that break down PBI cards into actionable work items.

### Task Card Template

#### Title Format
```
Task: [Short Description]
```

Example: `Task: Zen Quotes API Integration`

#### Description Template

```markdown
## Parent User Story

Issue #[NUMBER] - US[X]: [User Story Title]

## Task Description

[Detailed description of what this task involves]

## Subtasks

- [ ] [Subtask 1]
- [ ] [Subtask 2]
- [ ] [Subtask 3]
- [ ] [Additional subtasks...]

## Acceptance Criteria

- [ ] [Criterion 1]
- [ ] [Criterion 2]
- [ ] [Additional criteria specific to this task]

## Estimated Effort

[Hours or days]

## Technical Notes

[Any implementation details, API references, or technical considerations]

## Definition of Done

- [ ] Code written and follows project standards
- [ ] Code reviewed
- [ ] Tests written and passing
- [ ] Documentation updated
- [ ] No critical bugs
- [ ] Merged to main branch
```

### Creating Task Example: API Integration

**Step by step:**

1. Go to: Repository → Issues → New Issue
2. **Title**: `Task: Zen Quotes API Integration`
3. **Description**: (Following template above)
4. **Labels**: Add `Task`, `US6`, `Sprint 2`, `[Your Name]`
5. **Project**: Assign to "ToDo App - CSC305" project
6. **Column**: Place in "Sprint Backlog" initially
7. **Link to Parent**: In description, reference parent issue: `#6`
8. Click **Submit new issue**

**Full Example Description:**

```markdown
## Parent User Story

Issue #6 - US6: Inspirational Quotes

## Task Description

Research and implement integration with Zen Quotes API, including error handling and network resilience. This task establishes the backend connection to fetch inspirational quotes.

## Subtasks

- [ ] Research Zen Quotes API documentation and endpoints
- [ ] Set up API configuration in FlutterFlow
- [ ] Implement API call logic with proper error handling
- [ ] Add retry mechanism for failed requests
- [ ] Test API integration with various network conditions
- [ ] Implement fallback quotes for offline scenarios

## Acceptance Criteria

- [ ] Successfully fetches quotes from Zen Quotes API
- [ ] Handles API errors gracefully with user-friendly messages
- [ ] Implements retry logic for transient failures
- [ ] Works correctly with no network connection (fallback quotes)
- [ ] API calls are efficient and don't block UI
- [ ] Code is documented and follows project conventions

## Estimated Effort

4 hours

## Technical Notes

- API Endpoint: https://zenquotes.io/api/random
- No API key required for basic usage
- Response format: JSON array with quote and author
- Consider implementing caching to reduce API calls
- Use FlutterFlow API integration features

## Definition of Done

- [ ] Code written and follows project standards
- [ ] Code reviewed
- [ ] Tests written and passing
- [ ] Documentation updated
- [ ] No critical bugs
- [ ] Merged to main branch
```

---

## Workflow Management

### Moving Cards Between Columns

#### Sprint Planning Phase
1. Move selected PBI cards from **Product Backlog** → **Sprint Backlog**
2. Create task cards for each PBI
3. Move all task cards to **Sprint Backlog**
4. Ensure all cards have proper labels

#### During Sprint Execution
1. When starting work on a task: **Sprint Backlog** → **In Progress**
2. Update task with progress notes and checkmarks
3. When task is complete: **In Progress** → **Done**
4. When all tasks for a PBI are done, move PBI to **Done**

#### Sprint Completion
1. Verify all cards are in **Done**
2. Take screenshots for documentation
3. Conduct sprint retrospective
4. Plan next sprint

### Linking Issues

**Parent-Child Relationships:**
- In task issue description, reference parent: `Parent: #6` or `Closes #6`
- In parent PBI, list child tasks with checkboxes
- Use GitHub's "Development" section to link PRs to issues

**Cross-References:**
- Use `#[issue_number]` to reference related issues
- GitHub will automatically create backlinks

---

## Sprint 1 Setup (Retrospective)

Since Sprint 1 is complete, all cards should be in the **Done** column.

### PBI Cards for Sprint 1

Create 5 PBI issues (US1-US5) following the template above:

1. **Issue #1**: `To-Do-App #1 - US1: Account Creation`
   - Labels: `US1`, `Sprint 1`, `[Your Name]`, `PBI`
   - Column: **Done**

2. **Issue #2**: `To-Do-App #2 - US2: Login/Create Page`
   - Labels: `US2`, `Sprint 1`, `[Your Name]`, `PBI`
   - Column: **Done**

3. **Issue #3**: `To-Do-App #3 - US3: User Profile Editing`
   - Labels: `US3`, `Sprint 1`, `[Your Name]`, `PBI`
   - Column: **Done**

4. **Issue #4**: `To-Do-App #4 - US4: Dashboard`
   - Labels: `US4`, `Sprint 1`, `[Your Name]`, `PBI`
   - Column: **Done**

5. **Issue #5**: `To-Do-App #5 - US5: Checkout Page`
   - Labels: `US5`, `Sprint 1`, `[Your Name]`, `PBI`
   - Column: **Done**

### Task Cards for Sprint 1

Create 2-3 task cards for each PBI (10-15 total tasks):

**US1 Tasks:**
- Design registration form UI
- Implement backend validation
- Add secure password storage

**US2 Tasks:**
- Create login page UI
- Implement authentication logic
- Add session management

**US3 Tasks:**
- Design profile editing interface
- Implement update functionality
- Test profile updates

**US4 Tasks:**
- Design dashboard layout
- Implement CRUD operations
- Add filtering/sorting
- Integrate real-time updates

**US5 Tasks:**
- Create checkout page UI
- Implement confirmation logic
- Add navigation flow

All Sprint 1 tasks should be:
- Labeled with `Task`, appropriate `US#`, `Sprint 1`, `[Your Name]`
- Placed in **Done** column
- Marked as closed

---

## Sprint 2 Setup (Current)

Sprint 2 is currently in progress with US6.

### Creating Sprint 2 Cards

#### Step 1: Create US6 PBI Card

Follow the PBI template above. Example provided in "Creating PBI Cards" section.

- **Issue #6**: `To-Do-App #6 - US6: Inspirational Quotes`
- **Labels**: `US6`, `Sprint 2`, `[Your Name]`, `PBI`
- **Initial Column**: Product Backlog
- **Move to**: Sprint Backlog when sprint starts
- **Move to**: In Progress when work begins
- **Move to**: Done when all tasks complete

#### Step 2: Create Task Cards for US6

Create 3 task issues:

**Issue #7**: `Task: Zen Quotes API Integration`
- Labels: `Task`, `US6`, `Sprint 2`, `[Your Name]`
- Description: Reference issue #6 as parent
- Workflow: Sprint Backlog → In Progress → Done

**Issue #8**: `Task: Quote Display UI`
- Labels: `Task`, `US6`, `Sprint 2`, `[Your Name]`
- Description: Reference issue #6 as parent
- Workflow: Sprint Backlog → In Progress → Done

**Issue #9**: `Task: Testing & FlutterFlow Branch Merge`
- Labels: `Task`, `US6`, `Sprint 2`, `[Your Name]`
- Description: Reference issue #6 as parent
- Workflow: Sprint Backlog → In Progress → Done

#### Step 3: Link Tasks to Parent PBI

In issue #6 (US6 PBI), update the description to include:

```markdown
## Tasks

- [ ] Task: Zen Quotes API Integration (#7)
- [ ] Task: Quote Display UI (#8)
- [ ] Task: Testing & FlutterFlow Branch Merge (#9)
```

As each task is completed, check off the box in the parent PBI.

---

## Best Practices

### Card Management

1. **Be Specific**: Use clear, descriptive titles
2. **Keep Updated**: Update task progress regularly with comments
3. **Link Related Work**: Reference related issues and PRs
4. **Use Checklists**: Break work into subtasks with checkboxes
5. **Document Blockers**: Note any impediments in issue comments

### Label Discipline

1. **Always Label**: Every issue should have all applicable labels
2. **Consistent Naming**: Follow the label conventions established
3. **Color Coding**: Use consistent colors for similar label types
4. **Don't Over-Label**: Only use labels that add meaningful categorization

### Workflow Hygiene

1. **One Column at a Time**: Cards should only be in one column
2. **Move Cards Promptly**: Update board position when status changes
3. **Close When Done**: Close issues when work is verified complete
4. **Comment on Changes**: Explain significant status changes in comments
5. **Regular Updates**: Update board at least daily during active sprint

### Communication

1. **Use @mentions**: Tag team members in comments when needed
2. **Document Decisions**: Record important decisions in issue comments
3. **Link to Resources**: Reference documentation, PRs, and external resources
4. **Be Transparent**: Share blockers and challenges openly

---

## Screenshots and Evidence

Take screenshots at the following stages to document your workflow:

### Required Screenshots

1. **Sprint Backlog State**
   - Capture: All Sprint 2 cards in Sprint Backlog column
   - Shows: Initial sprint planning with all cards properly labeled

2. **In Progress State**
   - Capture: Cards actively being worked on
   - Shows: At least one task moved to In Progress column

3. **Done State - Partial**
   - Capture: Some tasks completed, others in progress
   - Shows: Progress through the sprint

4. **Done State - Complete**
   - Capture: All Sprint 2 cards in Done column
   - Shows: Sprint completion

5. **Labels View**
   - Capture: All labels created and properly configured
   - Shows: Complete label taxonomy

6. **Individual Card Examples**
   - Capture: US6 PBI card with full description
   - Capture: One task card showing parent linkage
   - Shows: Proper card formatting and relationships

### Screenshot Tips

- Use high resolution (1920x1080 or better)
- Ensure all relevant labels are visible
- Include project board URL in documentation
- Annotate screenshots if needed to highlight key elements
- Name files descriptively (e.g., `sprint2-backlog.png`)

---

## Troubleshooting

### Common Issues

#### Issue: Can't Add Card to Project
**Solution**: Ensure issue is created first, then add to project via issue sidebar or project board interface

#### Issue: Labels Not Showing
**Solution**: Verify labels are created at repository level (not project level) and properly applied to issues

#### Issue: Cards Not Linking
**Solution**: Use `#[number]` syntax to create references, ensure issues are in same repository

#### Issue: Column Organization Confused
**Solution**: Review workflow section, ensure understanding of backlog vs in-progress vs done

#### Issue: Missing Task Cards
**Solution**: Verify each PBI has 2-3 child tasks created, properly labeled and referenced

### Getting Help

- **GitHub Documentation**: https://docs.github.com/en/issues/planning-and-tracking-with-projects
- **Repository README**: Check README.md for project-specific guidance
- **Course Resources**: Refer to CSC305 course materials
- **Instructor Office Hours**: Reach out for project-specific questions

---

## Project Board URL

After setup, your project board will be accessible at:
```
https://github.com/juanvallejo97/To-Do-App/projects/[PROJECT_NUMBER]
```

**To find your project number:**
1. Go to your repository's Projects tab
2. Click on your project board
3. Look at the URL in your browser's address bar
4. The number after `/projects/` is your project number (e.g., if URL is `.../projects/3`, your number is 3)

Replace `[PROJECT_NUMBER]` with the actual number assigned by GitHub.

---

## Checklist for Complete Setup

Use this checklist to verify your project board is properly configured:

### Initial Setup
- [ ] Project board created with name "ToDo App - CSC305"
- [ ] Four columns created: Product Backlog, Sprint Backlog, In Progress, Done
- [ ] All labels created (US1-US6, Sprint 1-2, PBI, Task, [Your Name])

### Sprint 1 (Retrospective)
- [ ] 5 PBI cards created for US1-US5
- [ ] All Sprint 1 PBI cards labeled correctly
- [ ] 10-15 task cards created for Sprint 1 user stories
- [ ] All Sprint 1 task cards labeled correctly
- [ ] All Sprint 1 cards in Done column
- [ ] All Sprint 1 issues closed

### Sprint 2 (Current)
- [ ] 1 PBI card created for US6
- [ ] US6 PBI card labeled correctly
- [ ] 3 task cards created for US6
- [ ] All Sprint 2 task cards labeled correctly
- [ ] Task cards reference parent PBI (#6)
- [ ] Parent PBI lists child tasks with checkboxes
- [ ] Cards positioned correctly for current sprint state

### Documentation
- [ ] Screenshots taken at key workflow stages
- [ ] Project board URL documented
- [ ] USER_STORIES.md reviewed and referenced
- [ ] SPRINT_1.md reviewed for retrospective context
- [ ] SPRINT_2.md updated with current progress

---

## Summary

This guide provides everything needed to set up and manage the GitHub Project Board for the CSC305 ToDo App. Follow the templates, maintain discipline with labels and workflow, and document progress with screenshots.

**Key Takeaways:**
- Use consistent naming and labeling conventions
- Break user stories into actionable tasks
- Move cards through workflow columns as work progresses
- Link parent and child issues for traceability
- Document sprint progress with screenshots and updates
- Follow agile principles with regular updates and retrospectives

---

*Last updated: November 2025*  
*For CSC305 ToDo App Project*
