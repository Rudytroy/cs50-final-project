# To-Do App

## Video Demo: 
https://youtu.be/ol_AfDRJERM

## Description
This project is a simple web-based To-Do application built as the final project for the CS50x course.
The application allows users to add tasks, mark them as completed, and delete them.
All tasks are stored in a SQLite database, ensuring data persistence.

The goal of this project is to demonstrate understanding of backend development using Python and Flask,
basic database operations with SQLite, and dynamic HTML rendering with Jinja templates.

## Features
- Add new tasks
- View all tasks
- Mark tasks as completed
- Delete tasks
- Persistent storage using SQLite

## Technologies Used
- Python
- Flask
- SQLite
- HTML
- CSS

## Files Structure
project/
│
├── app.py
├── tasks.db
├── README.md
│
├── templates/
│ └── index.html
│
└── static/
└── style.css

## How to Run the Project
1. Make sure Python 3 is installed.
2. Install Flask:
python -m pip install flask
3. Run the application:
python app.py
4. Open a web browser and go to:
http://127.0.0.1:5000

## Design Decisions
- Flask was chosen for its simplicity and ease of use.
- SQLite was used as it is lightweight and does not require a separate server.
- The interface was kept minimal to focus on functionality rather than complex design.

## Author
Rudy Morillo

## Acknowledgements
This project was developed as part of Harvard University's CS50x course.