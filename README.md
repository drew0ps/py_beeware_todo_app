📝 ToDo App – BeeWare + Toga + SQLite

A simple, cross-platform desktop ToDo application built with BeeWare using the Toga GUI toolkit and SQLite via SQLAlchemy.

⸻

✨ Features
- Add new tasks with a simple user interface
- Tasks are stored persistently using a local SQLite database
- Clean, styled UI with a blue color palette
- Built entirely in Python, runs on macOS, Windows, Linux, and mobile (via BeeWare)

⸻

🛠 Requirements
- Python 3.8 or higher
- Toga
- SQLAlchemy
- BeeWare Briefcase

⸻

📦 Installation

1.	Clone the repository
	```
	git clone https://github.com/yourusername/toga-todo-app.git
	cd toga-todo-app
	```
2.	Create and activate a virtual environment
	```
	python -m venv venv
	source venv/bin/activate
	(On Windows: venv\Scripts\activate)
	```
3.	Install dependencies
	```
	pip install toga sqlalchemy
	```
4.	Run the app
	```
	briefcase dev 
	or
	briefcase run
	```



💾 Data Storage

The app uses a local SQLite database stored in the platform’s data directory:
- macOS: ~/Library/Application Support/{PATH}/todos.db
- Linux: ~/.local/share/{PATH}/todos.db
- Windows: %APPDATA%<AppName>\todos.db

⸻

🧠 How It Works
- On startup, the app loads all tasks saved in the SQLite database
- You can enter a new task in the text field and click Add task
- Each task is displayed in a scrollable container
- Tasks are stored immediately in the database after being added

⸻

🧹 Future Improvements
- Delete tasks
- Mark tasks as completed
- Add due dates and categories
- Theme switcher (dark/light mode)
- Package into a standalone app using BeeWare Briefcase
