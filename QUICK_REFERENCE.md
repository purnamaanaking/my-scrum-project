# Quick Reference Guide

## Creating Issues

### Create a User Story
```
Title: [USER STORY]: User can login to the system
Labels: user-story, priority-high
```

### Create a Task
```
Title: [TASK]: Implement authentication service
Labels: task, priority-medium
Related to: #123 (user story)
```

### Create a Bug
```
Title: [BUG]: Login button not responding
Labels: bug, priority-high
```

### Create an Epic
```
Title: [EPIC]: User Management System
Labels: epic, priority-high
```

## Project Board Workflow

```
Product Backlog → Sprint Backlog → In Progress → In Review → Done
```

1. **Product Backlog**: All items waiting to be prioritized
2. **Sprint Backlog**: Items committed for current sprint
3. **In Progress**: Actively being worked on
4. **In Review**: Code review or testing
5. **Done**: Completed and merged

## Sprint Workflow

### Week 1: Sprint Planning
- [ ] Review product backlog
- [ ] Estimate story points
- [ ] Create sprint milestone
- [ ] Move items to sprint backlog
- [ ] Set sprint goal

### Week 2-3: Development
- [ ] Daily standup (update board)
- [ ] Move items through workflow
- [ ] Update issue comments
- [ ] Create PRs and link to issues

### Week 4: Sprint Review & Retro
- [ ] Demo completed work
- [ ] Close completed issues
- [ ] Sprint retrospective
- [ ] Update velocity metrics
- [ ] Plan next sprint

## Common Commands

### Link Issues
```
Closes #123
Fixes #456
Related to #789
Blocks #101
Blocked by #102
```

### Mention Team Members
```
@username Can you review this?
cc @team-lead
```

### Add to Project
Issues are automatically added to the project when created.

## Story Point Reference

| Points | Complexity | Time Estimate |
|--------|------------|---------------|
| 1      | Trivial    | < 2 hours     |
| 2      | Simple     | 2-4 hours     |
| 3      | Moderate   | 4-8 hours     |
| 5      | Complex    | 1-2 days      |
| 8      | Very Complex | 2-4 days    |
| 13     | Large      | 1 week        |
| 21     | Very Large | 2 weeks       |

## Useful Links

- [Projects Board](../../projects)
- [Issues](../../issues)
- [Pull Requests](../../pulls)
- [Milestones](../../milestones)
- [Projects Guide](PROJECTS_GUIDE.md)

## Keyboard Shortcuts (GitHub)

- `c` - Create new issue
- `g` + `p` - Go to pull requests
- `g` + `i` - Go to issues
- `/` - Focus search
- `?` - Show keyboard shortcuts

## Git Workflow

```bash
# Start working on a story
git checkout -b feature/user-login

# Make changes and commit
git add .
git commit -m "feat: implement user login (#123)"

# Push and create PR
git push -u origin feature/user-login

# In PR description, link to issue:
# Closes #123
```

## Definition of Done

- [ ] Code written and follows style guide
- [ ] Unit tests written and passing
- [ ] Code reviewed and approved
- [ ] Integration tests passing
- [ ] Documentation updated
- [ ] PR merged to main branch
- [ ] Issue closed

## Common Labels

| Label | Use Case |
|-------|----------|
| `epic` | Large features |
| `user-story` | User stories |
| `task` | Technical tasks |
| `bug` | Bugs |
| `blocked` | Work is blocked |
| `in-progress` | Being worked on |
| `in-review` | In code review |
| `priority-high` | High priority |
| `priority-medium` | Medium priority |
| `priority-low` | Low priority |

---

💡 **Pro Tip**: Keep your project board updated daily for better visibility!
