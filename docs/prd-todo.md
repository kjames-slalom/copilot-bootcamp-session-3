# Product Requirements Document (PRD) - TODO App Upgrade

## 1. Overview

We are upgrading the existing TODO app to make task management more useful while keeping the implementation simple and teachable for the bootcamp. The product goal is to add lightweight planning features centered on due dates, task priority, and quick filtering, while keeping persistence local and avoiding backend changes for the MVP.

---

## 2. MVP Scope

- Add an optional `dueDate` field to each task using ISO `YYYY-MM-DD` format.
- Add a `priority` field to each task with allowed values `P1`, `P2`, and `P3`.
- Default `priority` to `P3` when a task is created without an explicit priority.
- Provide task filters for `All`, `Today`, and `Overdue`.
- Show completed tasks in the `All` filter.
- Exclude completed tasks from the `Today` and `Overdue` filters.
- Keep storage local only.
- Do not make backend or external storage changes as part of MVP.
- Require `title` for task creation and editing.
- Treat invalid `dueDate` values as absent instead of failing or storing bad data.
- Keep the overall experience simple and focused on core task organization.

---

## 3. Post-MVP Scope

- Visually highlight overdue tasks so they stand out in the task list.
- Add sorting rules so tasks are ordered by overdue status first, then by priority (`P1` to `P3`), then by due date ascending, with tasks that do not have a due date placed last.

---

## 4. Out of Scope

- Notifications
- Recurring tasks
- Multi-user support
- Keyboard navigation enhancements
- External storage
