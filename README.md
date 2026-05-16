# Python Todo List

A simple yet powerful command-line todo list application built with Python and SQLite. This project demonstrates how to manage tasks efficiently using a local database, with features to add, edit, mark tasks as complete, and display all tasks.

## Features

- ✅ **Add Tasks** - Easily add new tasks to your todo list
- ✏️ **Edit Tasks** - Modify existing tasks with updated descriptions
- ✔️ **Mark Complete** - Mark tasks as complete/incomplete
- 📋 **Display All Tasks** - View all tasks with their completion status
- 💾 **Persistent Storage** - All tasks are saved in a SQLite database

## Project Structure

```
Python-todo-list/
├── todolist.py      # Main application script
├── todo.db          # SQLite database file (auto-created)
└── README.md        # This file
```

## Requirements

- Python 3.x
- SQLite3 (usually included with Python)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/mahsajameei/Python-todo-list.git
cd Python-todo-list
```

2. No external dependencies required! SQLite3 is built into Python.

## Usage

Run the application:
```bash
python todolist.py
```

### Available Functions

#### Add a Task
```python
add_task("Your task description")
```

#### Edit a Task
```python
edit_task(task_id, "Updated task description")
```

#### Mark Task as Complete
```python
complete_task(task_id)
```

#### Display All Tasks
```python
display_tasks()
```

### Example Output
```
1 Bench Press 100 KG Completed
2 Deadlift 100 KG Completed
3 Squat 100 KG Completed
4 Dip 80 KG Completed
5 Pull Up 50 KG Incomplete
```

## How It Works

The application uses SQLite to manage a `tasks` table with the following structure:

- **id**: Unique identifier (auto-incremented)
- **task**: Task description
- **completed**: Status flag (0 = Incomplete, 1 = Complete)

All changes are immediately committed to the database, ensuring data persistence between sessions.

## Customization

You can easily modify the script to:
- Add a command-line interface (CLI) for interactive use
- Implement delete task functionality
- Add task priority levels
- Filter tasks by completion status
- Export tasks to different formats

## Future Enhancements

- [ ] Interactive command-line menu
- [ ] Delete task functionality
- [ ] Task priorities/categories
- [ ] Due dates for tasks
- [ ] Web interface with Flask/Django
- [ ] Data export (CSV, JSON)

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to fork this repository and submit pull requests with improvements!

## Author

**Mahsa Jameei**  
GitHub: [@mahsajameei](https://github.com/mahsajameei)

---

*Created: May 16, 2026*
