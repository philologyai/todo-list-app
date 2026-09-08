# To-Do List App

A simple, elegant to-do list application with local storage functionality. Create, manage, and organize your tasks with ease.

## Features

✨ **Core Functionality**
- ➕ Add new tasks
- ✅ Mark tasks as completed
- ❌ Delete tasks
- 🗑️ Clear all completed tasks

🎯 **Filtering**
- View all tasks
- View only active tasks
- View only completed tasks

💾 **Local Storage**
- Automatically saves tasks to browser's local storage
- Tasks persist across browser sessions
- No backend server required

🎨 **User Experience**
- Clean, modern interface with gradient design
- Smooth animations and transitions
- Responsive design for mobile and desktop
- Real-time task counter
- Confirmation dialogs for destructive actions

## How to Use

1. **Open the Application**: Open `index.html` in your web browser
2. **Add a Task**: 
   - Type your task in the input field
   - Click "Add Task" or press Enter
3. **Manage Tasks**:
   - Check the checkbox to mark a task as completed
   - Click "Delete" to remove a task
4. **Filter Tasks**: Use the filter buttons to view specific task types
5. **Clear Completed**: Remove all completed tasks at once

## Technical Details

### Technologies Used
- **HTML5**: Structure and semantic markup
- **CSS3**: Modern styling with flexbox and gradients
- **JavaScript ES6+**: Application logic and DOM manipulation
- **Local Storage API**: Persistent data storage

### File Structure
```
todo-list-app/
├── index.html       # Main HTML structure
├── styles.css       # Styling and animations
├── script.js        # Application logic
└── README.md        # Documentation
```

### Class: TodoApp

The application uses an object-oriented approach with a `TodoApp` class that manages:
- Task CRUD operations (Create, Read, Update, Delete)
- Local storage interactions
- DOM rendering and updates
- Event handling
- Filtering logic

#### Key Methods
- `addTodo()`: Add a new task
- `toggleTodo(id)`: Mark task as completed/active
- `deleteTodo(id)`: Remove a task
- `clearCompletedTodos()`: Remove all completed tasks
- `render()`: Update the DOM based on current state
- `saveToStorage()`: Persist tasks to local storage
- `loadFromStorage()`: Retrieve tasks from local storage
- `getFilteredTodos()`: Return filtered task list

## Data Structure

Each todo item is stored as an object:
```javascript
{
  id: 1234567890,           // Unique timestamp-based ID
  text: "Task description",  // Task text content
  completed: false,         // Completion status
  createdAt: "2024-01-15 10:30:45" // Creation timestamp
}
```

## Browser Compatibility

- Chrome/Edge: Full support
- Firefox: Full support
- Safari: Full support
- IE11: Requires polyfills for ES6+ features

## Local Storage Limits

- Storage limit: ~5-10MB per domain (varies by browser)
- Current implementation: Minimal storage footprint
- Suitable for hundreds of tasks without issues

## Customization

You can easily customize:
- **Colors**: Modify CSS gradient values in `styles.css`
- **Storage Key**: Change `storageKey` in `script.js`
- **Placeholder Text**: Update input placeholder in `index.html`
- **Animations**: Adjust CSS keyframes for different effects

## Future Enhancements

- 📅 Due date functionality
- 🏷️ Task categories/tags
- 🔍 Task search functionality
- 📊 Statistics and analytics
- 🌙 Dark mode toggle
- 🔄 Undo/Redo functionality
- ☁️ Cloud sync with backend
- 📱 Progressive Web App (PWA)

## License

MIT License - Feel free to use this project for personal or commercial purposes.

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest improvements
- Submit pull requests

## Support

If you encounter any issues:
1. Clear your browser cache
2. Check browser console for errors (F12)
3. Verify local storage is enabled in your browser
4. Try a different browser to test

Enjoy organizing your tasks! 🚀