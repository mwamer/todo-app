# To-Do List Application

A modern, feature-rich to-do list application built with vanilla HTML, CSS, and JavaScript. Manage your tasks efficiently with persistent local storage functionality.

## ✨ Features

### Core Functionality
- ✅ **Add Tasks** — Create new to-do items with a simple input interface
- ✅ **Mark Complete** — Check off completed tasks
- ✅ **Edit Tasks** — Modify existing tasks
- ✅ **Delete Tasks** — Remove individual tasks
- ✅ **Filter Tasks** — View all, active, or completed tasks
- ✅ **Clear Operations** — Remove completed or all tasks at once

### Advanced Features
- 💾 **Local Storage** — Tasks automatically save to your browser
- 📊 **Statistics** — View total, completed, and remaining task counts
- 🎨 **Responsive Design** — Works seamlessly on desktop, tablet, and mobile
- 🚀 **Smooth Animations** — Fluid transitions and interactive feedback
- ♿ **Accessibility** — Keyboard navigation and ARIA labels
- 💬 **Notifications** — Real-time feedback for user actions
- 🔒 **XSS Protection** — Secure HTML escaping

## 🚀 Getting Started

### Local Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mwamer/todo-app.git
   cd todo-app
   ```

2. **Open in browser:**
   - Simply open `index.html` in your web browser
   - No build process or dependencies required

3. **Start using:**
   - Enter a task in the input field
   - Press Enter or click "Add Task"
   - Your tasks are automatically saved

### Deployment with GitHub Pages

1. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Select `main` branch as source
   - Your app will be live at `https://mwamer.github.io/todo-app`

2. **Alternative hosting:**
   - Netlify, Vercel, or any static hosting service
   - Simply point to the repository

## 📱 Usage Guide

### Adding Tasks
1. Type your task in the input field
2. Press Enter or click the "Add Task" button
3. Task appears at the top of your list
4. Changes are saved automatically

### Managing Tasks
- **Mark Complete:** Click the checkbox next to a task
- **Edit Task:** Click the pencil (✎) icon to modify
- **Delete Task:** Click the trash (🗑) icon to remove

### Filtering Tasks
- **All** — View all tasks regardless of status
- **Active** — Show only incomplete tasks
- **Completed** — Show only finished tasks

### Statistics
- **Total Tasks** — Count of all tasks
- **Completed** — Number of finished tasks
- **Remaining** — Number of incomplete tasks

### Bulk Actions
- **Clear Completed** — Remove all finished tasks
- **Clear All** — Delete all tasks (with confirmation)

## 🛠️ Technology Stack

### Frontend
- **HTML5** — Semantic markup
- **CSS3** — Modern styling with CSS variables
- **JavaScript (ES6+)** — Vanilla JavaScript, no frameworks

### Storage
- **Local Storage API** — Persistent browser storage
- **JSON** — Data serialization

### Features Used
- CSS Grid & Flexbox for layout
- CSS Animations & Transitions
- JavaScript Classes & Methods
- Event Delegation
- DOM Manipulation
- Local Storage API

## 📂 Project Structure

```
todo-app/
├── index.html       # Main HTML structure
├── styles.css       # Styling and animations
├── app.js           # Application logic and functionality
└── README.md        # Documentation
```

### File Descriptions

#### `index.html`
- Semantic HTML5 structure
- Form elements with accessibility attributes
- Statistics display
- Filter buttons
- Action buttons
- Task list container

#### `styles.css`
- CSS custom properties (variables)
- Responsive grid and flexbox layouts
- Smooth animations and transitions
- Color scheme and typography
- Mobile-first design approach
- Dark mode ready

#### `app.js`
- `TodoApp` class with all functionality
- Local storage integration
- DOM manipulation and rendering
- Event handling
- Data validation
- Notification system

## 🎨 Design Highlights

### Color Scheme
- **Primary:** Blue (#2563EB) for main actions
- **Success:** Green (#10B981) for completions
- **Warning:** Orange (#F59E0B) for confirmations
- **Danger:** Red (#EF4444) for deletions

### Typography
- **Font:** System fonts (-apple-system, Segoe UI, etc.)
- **Base Size:** 16px
- **Line Height:** 1.75 for readability

### Animations
- Slide-in animations for new tasks
- Smooth color transitions
- Hover effects for interactivity
- Fade-out for deleted items

## ⌨️ Keyboard Shortcuts

- **Enter** — Add new task (when input is focused)
- **Tab** — Navigate between elements
- **Shift + Tab** — Navigate backward
- **Space** — Toggle checkbox when focused

## 📊 Data Storage

### Local Storage Format
```json
[
  {
    "id": 1693478400000,
    "text": "Sample task",
    "completed": false,
    "createdAt": "2023-08-30T12:00:00.000Z"
  }
]
```

### Storage Key
- Default key: `todoAppData`
- Modifiable in `app.js` constructor

### Storage Limitations
- Browser local storage: ~5-10MB per domain
- Persistent across browser sessions
- Cleared when browser data is cleared

## 🔒 Security Features

- HTML escaping to prevent XSS attacks
- Input validation
- Confirmation dialogs for destructive actions
- No external dependencies or vulnerable packages

## ♿ Accessibility

- **WCAG 2.1 Level AA** compliant
- Semantic HTML elements
- ARIA labels for screen readers
- Keyboard navigation support
- High contrast mode support
- Focus-visible states
- Readable font sizes

## 🚀 Performance

- **No external dependencies** — Lightweight and fast
- **Minimal DOM updates** — Efficient rendering
- **CSS-based animations** — Smooth 60fps performance
- **Optimized for mobile** — Fast loading and interaction
- **Small file size** — ~15KB total (uncompressed)

## 🌐 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Internet Explorer 11+ (limited support)

## 🔧 Customization

### Change Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #2563EB;
    --success-color: #10B981;
    /* ... more variables ... */
}
```

### Change Storage Key
Modify in `app.js`:
```javascript
this.storageKey = 'myCustomKey';
```

### Add More Features
- Due dates for tasks
- Priority levels
- Categories/tags
- Search functionality
- Dark mode toggle
- Multiple lists/projects

## 📝 Future Enhancements

- [ ] Due date functionality
- [ ] Priority levels
- [ ] Task categories/tags
- [ ] Search and filter by text
- [ ] Dark mode toggle
- [ ] Multiple lists/projects
- [ ] Cloud synchronization
- [ ] Recurring tasks
- [ ] Time tracking
- [ ] Task notes/descriptions

## 🐛 Troubleshooting

### Tasks not saving?
- Check if local storage is enabled in your browser
- Verify browser isn't in private/incognito mode
- Check browser console for errors

### Tasks disappeared?
- Clearing browser data will delete local storage
- Try refreshing the page
- Check if another tab has the app open

### Performance issues?
- Clear completed tasks regularly
- Reduce number of tasks (though app handles 1000+)
- Try a different browser

## 📄 License

Open source - free to use and modify

## 👥 Contributing

Feel free to fork, modify, and submit improvements!

## 📞 Support

For issues or questions:
- Open a GitHub issue
- Check existing issues first
- Provide detailed description and steps to reproduce

## 🎉 Credits

Built with vanilla JavaScript - no frameworks or external libraries.

---

**Last Updated:** August 27, 2026

**Start organizing your tasks today!** 🚀
