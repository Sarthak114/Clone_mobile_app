**Working of the To-Do List APK (Step by Step)**

1. Launching the App
   
When you tap the app icon, Android loads the APK (compiled version of your Flutter code).
main() function runs → it executes runApp(const ToDoApp());.
This sets up the root widget ToDoApp with MaterialApp design..

2. Home Screen Layout

The screen (ToDoHome) is divided into two main parts:
Input Section (Top)
A TextField with placeholder text → "Enter task...".
A plus (+) icon button next to it.
Task List Section (Bottom)
An empty list area when you first open the app (since _tasks list is empty).
This space is scrollable because of ListView.builder.

3. Viewing the List

Every time you add a task, a new ListTile is created inside the list.
Example after adding 3 tasks:
Buy groceries 🛒
Study Flutter 📘
Call Mom 📞
Each row contains:
Task text on the left.
A red delete icon (trash can) on the right.

4. Removing a Task

When you tap the red delete icon next to a task → _removeTask(index) runs.
The task at that index is removed from _tasks.
setState() triggers UI refresh.
Result: That task disappears instantly from the list.

5. Continuous Use

You can repeat:
Typing in new tasks.
Adding them with the + button.
Deleting any task with the red trash button.
