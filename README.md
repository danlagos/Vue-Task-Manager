# Task Manager App Overview
This app allows users to add, delete, and categorize tasks. Users can also mark tasks as completed or important, and filter tasks based on their status or category.

## App Structure
- **Main Component:** Holds the state of all tasks and includes methods for adding, deleting, and updating tasks.
- **TaskList Component:** Renders the list of tasks using `v-for`. Each task is a TaskItem component.
- **TaskItem Component:** Represents a single task. It can be clicked to toggle its completion status or marked as important.
- **AddTaskForm Component:** A form for adding new tasks with `v-model` for two-way data binding and basic validation to ensure the task name isn't empty.

## Features & Vue.js Concepts
1. **Attribute Binding**
   - Dynamically bind attributes, like image icons or links related to task categories.
2. **Conditional Rendering**
   - Use `v-if` or `v-show` to conditionally display tasks based on filters (e.g., show only completed tasks).
3. **List Rendering**
   - Use `v-for` to render a list of tasks that can be dynamically added or removed.
4. **Event Handling**
   - Handle adding new tasks, marking tasks as complete, or deleting them with button clicks.
5. **Class and Style Binding**
   - Bind classes or styles to tasks based on their status (e.g., a different color for completed tasks).
6. **Computed Properties**
   - Calculate and display stats like the number of active tasks or tasks per category.
7. **Components and Props**
   - Break the app into smaller components (e.g., TaskItem, TaskList, AddTaskForm) and pass necessary data using props.
8. **Communicating Events**
   - Use custom events to allow child components (like TaskItem) to notify the parent component of changes (e.g., task completion).
9. **v-model**
   - Use `v-model` in forms for adding tasks to bind input fields directly to the app's data.
10. **Forms and Validation**
    - Implement a form to add new tasks with validations to check for empty inputs or invalid formats.

## Additional Ideas
- Add the ability to save and load tasks from local storage.
- Implement filters to view tasks by status (all, active, completed) or by category (personal, work, etc.).
- Provide drag-and-drop sorting of tasks for prioritization.
