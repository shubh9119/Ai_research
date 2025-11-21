📘 Research Assistant — Web Version

A browser-based research assistant converted from the original Python/Tkinter desktop app.
This web version replicates the UI layout and provides a modern front-end using HTML, CSS, and JavaScript.

📁 Project Structure
project/
│
├── index.html        # Main HTML file (structure: sidebar, topbar, chat UI)
├── style.css         # All styles (layout, colors, dark mode)
├── script.js         # App logic (send messages, UI behavior, etc.)
│
└── assets/           # Images, icons, optional fonts
    └── icons/


Note: The structure may vary slightly based on how you organize your files.
If your code is all-in-one HTML, only index.html will exist.

🚀 Features

Modern sidebar + chat layout

Quick reply suggestion buttons

Chat bubbles with scrolling

Research workflow UI

Dark/Light theme styling

Modular file structure (HTML/CSS/JS)

🛠 Requirements

This web version does not require Python or any backend, unless you add API calls later.

Minimum Requirements

A modern browser (Chrome, Firefox, Edge, Safari)

A local HTTP server (optional but recommended)

Optional (if you plan to extend functionality)

Node.js (for bundling or hosting)

A backend API endpoint (if replacing Wikipedia API logic)

▶️ How to Run
Method 1 — Open directly (simple)

Just double-click:

index.html


This works if your JS does not require module imports or fetch calls to local files.

Method 2 — Run with a local web server (recommended)

Some browsers block features (like fetch()) unless served via HTTP.

If you have Python installed:
cd project
python3 -m http.server 8000


Open in browser:

http://localhost:8000

If you use Node.js:
npm install -g serve
serve .

⚙️ Customization
Change theme colors

Edit variables in style.css:

:root {
    --bg-color: #ffffff;
    --text-color: #000000;
    --accent-color: #475569;
}

Modify chat messages

Inside script.js, update:

addMessage("Hello! How can I help you?", "assistant");

Add API calls

Inside script.js, you can replace the placeholder function:

function fetchData(query) {
    // Add real API call here (Wikipedia, your own backend, etc.)
}

📦 Future Enhancements

Add backend API (Python Flask, FastAPI, Node.js, etc.)

Add user authentication

Save conversation history to localStorage or a database

Add animated loading steps

Integrate real research agents

📝 License

MIT License
Feel free to modify and use this project however you'd like.
