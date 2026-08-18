# To-Do List Application

A modern, fully-functional to-do list web application with persistent local storage, filtering capabilities, and an intuitive user interface.

## Features

### Core Functionality
- ✅ **Add Tasks**: Easily add new tasks with a single click or Enter key
- ✅ **Mark Complete**: Check off tasks as you complete them
- ✅ **Delete Tasks**: Remove individual tasks with a delete button
- ✅ **Clear Options**: Clear completed tasks or all tasks at once

### Organization & Filtering
- 🔍 **Filter by Status**: View All, Active, or Completed tasks
- 📊 **Live Statistics**: Real-time count of total, active, and completed tasks
- 🎯 **Priority Badges**: Visual indicators for task priority levels

### Data Persistence
- 💾 **Local Storage**: Automatically saves all tasks to browser storage
- 🔄 **Auto-Load**: Tasks persist across browser sessions and page refreshes
- 🛡️ **Error Handling**: Graceful fallback if storage is unavailable

### User Experience
- 📱 **Fully Responsive**: Works perfectly on desktop, tablet, and mobile devices
- ✨ **Smooth Animations**: Slide-in and slide-out animations for tasks
- 🎨 **Modern Design**: Beautiful gradient styling with smooth transitions
- ⌨️ **Keyboard Support**: Add tasks with Enter key for faster workflow

## How to Use

1. Open `todo.html` in your web browser
2. Enter a task name in the input field
3. Click "Add Task" or press Enter
4. Click the checkbox to mark tasks as complete
5. Use filters to view specific tasks
6. Click "Delete" to remove individual tasks
7. Use "Clear Completed" or "Clear All" for bulk operations

## File Structure

```
wamadat/
├── todo.html           # Main application HTML
├── styles/
│   └── todo.css       # Complete styling and animations
├── scripts/
│   └── todo.js        # Application logic and local storage
```

## Local Storage Implementation

The application uses the browser's `localStorage` API to persist tasks:

- **Storage Key**: `wamadat_todos`
- **Storage Format**: JSON array of todo objects
- **Data Structure**:
  ```javascript
  {
    id: timestamp,
    text: "Task description",
    completed: boolean,
    createdAt: "MM/DD/YYYY",
    priority: "high|medium|low"
  }
  ```

## Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Flexbox, Grid, Gradients, Animations
- **Vanilla JavaScript**: No external dependencies
- **Browser APIs**: LocalStorage API

## Features Breakdown

### Task Management
- Add new tasks with validation
- Toggle completion status
- Delete individual tasks
- View task creation date

### Filtering System
- All tasks
- Active tasks only
- Completed tasks only
- Dynamic filter button styling

### Statistics Dashboard
- Total tasks count
- Active tasks count
- Completed tasks count
- Real-time updates

### Storage System
- Automatic save after each action
- Persistent across sessions
- Error handling for storage failures
- Console logging for debugging

## Browser Support

Works in all modern browsers that support:
- ES6 JavaScript
- LocalStorage API
- CSS Grid and Flexbox
- HTML5 semantic elements

## Future Enhancements

- [ ] Task categories/tags
- [ ] Due dates and reminders
- [ ] Task descriptions/notes
- [ ] Custom priority levels
- [ ] Search functionality
- [ ] Keyboard shortcuts
- [ ] Dark mode
- [ ] Cloud sync with backend
- [ ] Task export/import
- [ ] Recurring tasks
- [ ] Drag and drop reordering
- [ ] Local notifications

## Installation

No installation required! Simply open `todo.html` in any modern web browser.

### For Local Development
```bash
# Clone the repository
git clone https://github.com/mohamedtaherradwan-alt/wamadat.git
cd wamadat

# Open in browser
open todo.html
# or
start todo.html
```

## Privacy & Data

- All tasks are stored locally in your browser
- No data is sent to any server
- Data persists until you manually clear it or clear browser cache
- Clearing browser storage will remove all saved tasks

## Troubleshooting

### Tasks not saving?
- Check if LocalStorage is enabled in your browser
- Try increasing your browser's storage quota
- Clear browser cache and try again

### Tasks disappearing?
- Ensure LocalStorage is enabled
- Check browser console for errors (F12)
- Tasks are cleared when you use "Clear All" button

## License

Open source - feel free to use, modify, and distribute

## Support

For issues or feature requests, please open an issue on GitHub.

---

**Wamadat To-Do List** - Stay organized and boost your productivity! 🚀
