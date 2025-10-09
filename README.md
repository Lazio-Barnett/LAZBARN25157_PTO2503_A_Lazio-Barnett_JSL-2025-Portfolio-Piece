# 📌 JSLPP – Kanban Task Board

## 🚀 Project Overview

This project builds a **dynamic Kanban Task Board** in the browser. Tasks are displayed in three columns: **TODO, DOING, DONE**, and can be added, edited, or deleted directly on the page.

Each task is stored as an object with its **id, title, description, and status**. Tasks are initially fetched from an API, with a **fallback to localStorage** if the API is unavailable. Clicking a task opens a **modal (pop-up)** for viewing and editing details. The board updates in real-time based on user interactions.

You can view a demo presentation here:
[📽️ JSLPP Kanban Presentation](https://www.veed.io/view/fbad54b0-6814-4421-85d5-4089f7f98226?source=Homepage&panel=share)

---

## ✨ Features

- Tasks stored as objects in an array
- Fetch tasks from API; fallback to localStorage if API fails
- Dynamic rendering of tasks in the correct column based on status
- Click task to open **edit modal** with title, description, and status
- Add new tasks through **new-task modal**
- Delete tasks with confirmation
- Modal can be closed with ✕, backdrop click, or **Esc**
- Dark/light theme toggle (desktop + mobile)
- Collapsible sidebar and mobile overlay menu
- Responsive layout: 3 columns on desktop → 2 on tablet → 1 on mobile

---

## 🛠️ Technologies Used

- **HTML5** – page structure for sidebar, header, board, and modals
- **CSS3** – styling for board layout, cards, modals, responsive design, and themes
- **JavaScript (ES6 Modules)** – modularized code for:

  - `main.js` → initialization, status banners, wiring UI
  - `api.js` → fetching tasks from API
  - `tasks/taskManager.js` → CRUD operations
  - `ui/` → modals, sidebar, mobile menu, theme, rendering tasks

---

## 📁 Project Structure

```
index.html             # Page structure: sidebar, header, board, modals
styles.css             # Styles: board layout, modals, theme, responsiveness
scripts/
├── main.js            # App initialization, wiring UI, status banner
├── api.js             # Fetch tasks from API with fallback
├── tasks/
│   └── taskManager.js # Add, update, delete tasks
└── ui/
    ├── render.js        # Render tasks to columns
    ├── taskElement.js   # Create individual task elements
    ├── modalHandlers.js # Add/edit modal functionality
    ├── sidebar.js       # Desktop collapsible sidebar
    ├── mobileMenu.js    # Mobile menu overlay
    └── theme.js         # Dark/light theme toggle
assets/                 # Logos, icons, favicon
README.md
```

---

## ▶️ How to Use

1. Open `index.html` in a browser
2. Tasks are fetched from the API or loaded from localStorage
3. Click **+ Add New Task** to open the add-task modal

   - Enter title, description, and select status
   - Click **Create Task** → new task appears in correct column

4. Click a task card to open the **edit modal**

   - Update title, description, or status
   - Click **Save changes** to update board immediately
   - Click **Delete task** to remove it (confirmation required)

5. Collapse sidebar or toggle theme (desktop + mobile)
6. Modal can be closed with ✕ button, backdrop click, or **Esc**

---

## ✅ User Stories Covered

- Fetch tasks from API; fallback to localStorage if unavailable
- Tasks render dynamically in correct column based on status
- Modals for editing tasks with validation (required fields)
- Add new tasks via modal; tasks saved in memory and storage
- Delete tasks with confirmation
- Responsive layout and collapsible sidebar
- Dark/light theme toggle
- Mobile-friendly menu and interactions

---

## 👤 Author

**Lazio Barnett**

- GitHub: [https://github.com/Lazio-Barnett](https://github.com/Lazio-Barnett)
- Presentation: [📽️ Watch here](https://www.veed.io/view/fbad54b0-6814-4421-85d5-4089f7f98226?source=Homepage&panel=share)
