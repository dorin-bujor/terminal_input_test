# Task Management System

## Objective
Create a Java application that demonstrates **console input handling** and **basic logic based on user input**. The application will simulate a simple **Task Management System** where users can:
1. Add a task.
2. View all tasks.
3. Mark a task as complete.
4. Delete a task.
5. Exit the program.

---

## Requirements

### 1. Task Class
Create a class `Task` with the following attributes:
- `id` (int) - unique identifier for the task.
- `description` (String) - description of the task.
- `isCompleted` (boolean) - indicates whether the task is completed.

Use encapsulation (private fields with getters and setters). Override the `toString()` method to return a formatted string representation of the task.

### 2. Main Application
Use a `List<Task>` to store all tasks. Implement a **menu-driven console application** with the following options:
1. **Add Task**:
   - Prompt the user to enter a task description.
   - Assign a unique ID to the task (auto-increment based on the list size).
   - Create a `Task` object and add it to the list.
2. **View All Tasks**:
   - Display all tasks in the list using the `toString()` method.
3. **Mark Task as Complete**:
   - Prompt the user to enter the task ID.
   - Mark the corresponding task as completed.
4. **Delete Task**:
   - Prompt the user to enter the task ID.
   - Remove the corresponding task from the list.
5. **Exit**:
   - Exit the program.

### 3. Input Validation
- Validate user input for task IDs (ensure the ID exists in the list).
- Handle invalid input gracefully (e.g., display an error message and prompt the user again).

---

### 4. Sample Output

=== Task Management System ===
1. Add Task
2. View All Tasks
3. Mark Task as Complete
4. Delete Task
5. Exit

Enter your choice: 1
Enter task description: Buy groceries
Task added successfully!

Enter your choice: 2
Tasks:
[ID: 1] Description: Buy groceries - Completed: false

Enter your choice: 3
Enter task ID to mark as complete: 1
Task marked as completed!

Enter your choice: 2
Tasks:
[ID: 1] Description: Buy groceries - Completed: true

Enter your choice: 4
Enter task ID to delete: 1
Task deleted successfully!

Enter your choice: 2
Tasks:
No tasks found.

Enter your choice: 5
Exiting the program. Goodbye!

