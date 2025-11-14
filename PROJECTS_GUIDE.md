# GitHub Projects Setup Guide

This document provides instructions on how to set up and use GitHub Projects for managing this Scrum project.

## Table of Contents
- [Setting Up a New Project Board](#setting-up-a-new-project-board)
- [Configuring the Project Board](#configuring-the-project-board)
- [Creating and Managing Issues](#creating-and-managing-issues)
- [Sprint Planning](#sprint-planning)
- [Daily Scrum](#daily-scrum)
- [Sprint Review and Retrospective](#sprint-review-and-retrospective)

## Setting Up a New Project Board

1. **Create a New Project**
   - Navigate to the repository on GitHub
   - Click on the "Projects" tab
   - Click "New project"
   - Select "Board" or "Table" view (Board view is recommended for Scrum)
   - Name your project (e.g., "Sprint 1", "Product Backlog", or "My Scrum Project")

2. **Choose a Template**
   - GitHub offers several templates:
     - **Basic Kanban**: Simple To Do, In Progress, Done columns
     - **Automated Kanban**: Same as Basic but with automation
     - **Bug Tracker**: For bug management
   - For Scrum, start with "Automated Kanban" and customize it

## Configuring the Project Board

### Recommended Columns for Scrum

1. **Product Backlog** - All user stories and tasks that are not yet committed to a sprint
2. **Sprint Backlog** - Items committed to the current sprint
3. **In Progress** - Items currently being worked on
4. **In Review** - Items in code review or testing
5. **Done** - Completed items (consider archiving after sprint review)

### Setting Up Automation

1. Click on the three dots (...) on each column
2. Select "Manage automation"
3. Configure automation rules:
   - **Sprint Backlog**: Automatically add newly created issues
   - **In Progress**: Move here when an issue is assigned
   - **In Review**: Move here when a PR is created
   - **Done**: Move here when a PR is merged or issue is closed

### Custom Fields (GitHub Projects V2)

Add custom fields to track Scrum-specific information:
- **Story Points**: Number field for effort estimation
- **Sprint**: Text or iteration field to track which sprint an item belongs to
- **Priority**: Single select (High, Medium, Low)
- **Type**: Single select (Epic, User Story, Task, Bug)

## Creating and Managing Issues

### Issue Types

This project includes templates for:
- **Epic** - Large features spanning multiple sprints
- **User Story** - Features from the user's perspective
- **Task** - Technical work items
- **Bug** - Issues to be fixed

### Creating an Issue

1. Go to the "Issues" tab
2. Click "New issue"
3. Choose the appropriate template
4. Fill in all required fields
5. Assign labels, projects, and assignees
6. Link to related issues (e.g., tasks to user stories, user stories to epics)

### Writing Good User Stories

Follow the format: "As a [type of user], I want [goal] so that [reason]"

Example:
```
As a registered user, I want to reset my password so that I can regain access to my account if I forget it.
```

### Acceptance Criteria

Each user story should have clear acceptance criteria:
```
- [ ] User can request password reset from login page
- [ ] System sends reset link to user's email
- [ ] Reset link expires after 24 hours
- [ ] User can set a new password using the link
- [ ] User receives confirmation after successful reset
```

## Sprint Planning

### Before Sprint Planning

1. **Backlog Refinement**
   - Review and prioritize items in the Product Backlog
   - Ensure user stories have:
     - Clear descriptions
     - Acceptance criteria
     - Story point estimates
   - Break down large items (epics) into smaller user stories

2. **Estimate Story Points**
   - Use Planning Poker or similar technique
   - Use Fibonacci sequence: 1, 2, 3, 5, 8, 13, 21
   - Consider complexity, effort, and uncertainty

### During Sprint Planning

1. **Set Sprint Goal**
   - Define what you want to achieve in the sprint
   - Create a milestone for the sprint

2. **Select Items for Sprint**
   - Team discusses and commits to user stories
   - Move items from Product Backlog to Sprint Backlog
   - Don't overcommit - leave buffer for unexpected issues

3. **Break Down User Stories**
   - Create tasks for each user story
   - Link tasks to their parent user story

4. **Set Sprint Dates**
   - Use GitHub Milestones to track sprint dates
   - Typically 1-4 weeks duration

## Daily Scrum

### Using GitHub for Daily Updates

1. **Review the Board**
   - Check items In Progress
   - Identify blockers (add "blocked" label)
   - Update issue status

2. **Comment on Issues**
   - Add daily progress updates to issues
   - Mention team members with @username
   - Document blockers and dependencies

3. **Update Assignees**
   - Assign yourself to new tasks
   - Unassign when moving to review

## Sprint Review and Retrospective

### Sprint Review

1. **Demo Completed Work**
   - Filter project board by "Done" status
   - Review each completed item
   - Get stakeholder feedback

2. **Update Product Backlog**
   - Add new items based on feedback
   - Reprioritize existing items

### Sprint Retrospective

1. **What Went Well**
   - Use GitHub Discussions or create an issue
   - Tag with "retrospective" label

2. **What Needs Improvement**
   - Document action items as GitHub issues
   - Assign owners for improvements

3. **Metrics to Review**
   - Velocity (story points completed)
   - Cycle time (time from start to done)
   - Number of bugs found
   - Items completed vs committed

## Best Practices

### Issue Management
- Keep issues atomic and focused
- Link related issues using keywords: "Related to #123", "Blocks #456", "Closes #789"
- Use clear, descriptive titles
- Update issues regularly
- Close issues when done

### Labels
Use labels consistently:
- **Type**: epic, user-story, task, bug
- **Priority**: high, medium, low
- **Status**: blocked, in-review, needs-discussion
- **Sprint**: sprint-1, sprint-2, etc.

### Project Board
- Review and update the board daily
- Archive old boards after sprint completion
- Keep descriptions up to date
- Use milestones for sprint tracking

### Collaboration
- @mention team members for collaboration
- Use PR reviews for code quality
- Link PRs to issues they resolve
- Keep communication in GitHub for traceability

## Additional Resources

- [GitHub Projects Documentation](https://docs.github.com/en/issues/planning-and-tracking-with-projects)
- [Scrum Guide](https://scrumguides.org/)
- [User Story Best Practices](https://www.mountaingoatsoftware.com/agile/user-stories)
- [GitHub Issues Documentation](https://docs.github.com/en/issues)

## Quick Start Checklist

- [ ] Create a new GitHub Project for your first sprint
- [ ] Set up project columns (Backlog, Sprint, In Progress, Review, Done)
- [ ] Create initial epics for major features
- [ ] Break down epics into user stories
- [ ] Add acceptance criteria to user stories
- [ ] Estimate story points for backlog items
- [ ] Plan your first sprint
- [ ] Set up automation rules
- [ ] Configure custom fields
- [ ] Create a sprint milestone

---

**Need Help?** Create an issue with the question label or start a discussion in GitHub Discussions.
