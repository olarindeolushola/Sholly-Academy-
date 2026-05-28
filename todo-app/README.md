# To-Do List Application

A simple, elegant to-do list application with local storage functionality.

## Features

✅ **Add Tasks** - Create new tasks with a simple input field  
✅ **Mark Complete** - Check off tasks as you complete them  
✅ **Delete Tasks** - Remove individual tasks  
✅ **Filter Tasks** - View all, active, or completed tasks  
✅ **Local Storage** - Tasks persist across browser sessions  
✅ **Statistics** - View total and completed task count  
✅ **Responsive Design** - Works on desktop and mobile  
✅ **Clear All** - Remove all completed or all tasks at once  

## How to Use

1. **Add a Task**
   - Type your task in the input field
   - Press Enter or click the "Add Task" button

2. **Complete a Task**
   - Click the checkbox next to the task to mark it complete
   - Completed tasks show a strikethrough effect

3. **Delete a Task**
   - Click the "Delete" button on any task

4. **Filter Tasks**
   - Use the filter buttons (All, Active, Completed) to view specific tasks

5. **Manage Tasks**
   - "Clear Completed" removes all completed tasks
   - "Delete All" removes all tasks (with confirmation)

## Local Storage

The application uses the browser's local storage to persist tasks. Your tasks are automatically saved and will be restored when you return to the application.

**Storage Key**: `sholly_academy_todos`

## Technical Details

### Technology Stack
- **HTML5** - Structure and markup
- **CSS3** - Styling and responsive design
- **JavaScript (ES6+)** - Application logic
- **Local Storage API** - Data persistence

### File Structure
```
todo-app/
├── index.html      # Main HTML file
├── styles.css      # Styling and responsive design
├── script.js       # Application logic
└── README.md       # Documentation
```

### Key Classes

#### TodoApp Class
Main class managing the entire application:
- `addTodo()` - Add a new task
- `deleteTodo(id)` - Delete a task by ID
- `toggleTodo(id)` - Mark task as complete/incomplete
- `clearCompleted()` - Remove all completed tasks
- `deleteAll()` - Remove all tasks
- `setFilter(filter)` - Change the current filter
- `saveToStorage()` - Save tasks to local storage
- `loadFromStorage()` - Load tasks from local storage
- `render()` - Update the UI

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Installation

Simply open `index.html` in your web browser. No installation or build process required!

```bash
# Option 1: Direct file opening
open index.html

# Option 2: Using a local server (Python)
python -m http.server 8000
# Then visit http://localhost:8000/todo-app

# Option 3: Using a local server (Node.js)
npx http-server
# Then visit http://localhost:8080/todo-app
```

## Data Structure

Each todo object has the following structure:

```javascript
{
    id: 1234567890,           // Unique identifier (timestamp)
    text: "Buy groceries",    // Task description
    completed: false,         // Completion status
    createdAt: "Date string" // Creation timestamp
}
```

## Future Enhancements

- Edit existing tasks
- Task categories/tags
- Due dates and reminders
- Task priority levels
- Export/import functionality
- Dark mode
- Cloud synchronization

## License

MIT License
