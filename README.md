# To-Do App

## Video Demo:
https://youtu.be/ol_AfDRJERM

## Introduction

This project is a web-based To-Do application developed as the final project for Harvard University's CS50x course.
The purpose of this project is to demonstrate an understanding of fundamental computer science concepts,
backend web development, and database management using practical tools and technologies.

The application allows users to manage a list of tasks by adding new tasks, marking them as completed,
and deleting them. Although the application is intentionally simple in terms of features, it was designed
to clearly showcase core programming concepts such as control flow, data persistence, CRUD operations,
and separation of concerns between backend logic and frontend presentation.

## Project Overview

The To-Do App provides a minimal yet functional interface where users can interact with a task list through a web browser.
Users can submit new tasks using a form, see all existing tasks displayed on the page, visually identify completed tasks,
and remove tasks that are no longer needed.

All data is stored in a SQLite database, ensuring that tasks persist even after the application is stopped or restarted.
This persistence was an important design requirement, as it demonstrates the use of databases instead of temporary in-memory storage.

## Technologies Used

The project was built using the following technologies:

- **Python**: Used as the primary programming language for backend logic.
- **Flask**: A lightweight web framework that handles routing, HTTP requests, and template rendering.
- **SQLite**: A file-based relational database used to store tasks.
- **HTML**: Used to structure the web page.
- **CSS**: Used to apply basic styling and improve usability.
- **Jinja**: Flask’s templating engine, used to dynamically render task data.

These technologies were chosen because they are well-suited for small-scale applications and align with the concepts taught throughout CS50x.

## File Structure and Explanation

The project is organized into the following structure:

project/
│
├── app.py
├── README.md
│
├── templates/
│ └── index.html
│
└── static/
└── style.css

### app.py

This is the main backend file of the application. It initializes the Flask app, establishes a connection to the SQLite database,
defines the database schema, and handles all routes.

The file includes routes for:
- Displaying all tasks
- Adding a new task
- Marking a task as completed
- Deleting a task

It also includes a database initialization function that ensures the required table exists before the application runs.
This design choice simplifies setup and prevents runtime errors if the database file does not already exist.

### templates/index.html

This file defines the structure of the web interface. It uses HTML combined with Jinja templating syntax to dynamically
display tasks retrieved from the database.

The template includes:
- A form for submitting new tasks
- A list that displays all tasks
- Visual indicators for completed tasks
- Action links to complete or delete tasks

Using Jinja allows the backend to pass data directly to the template, maintaining a clean separation between logic and presentation.

### static/style.css

This file contains all styling rules for the application. The CSS was intentionally kept simple to maintain focus on functionality.
Basic styling such as layout alignment, spacing, font selection, and hover effects were added to improve readability and usability.

Separating CSS into its own file follows best practices and keeps the HTML template clean and readable.

## Design Decisions

Several design decisions were made during development:

- **No user authentication**: Authentication was intentionally excluded to keep the scope manageable and focus on core concepts.
- **SQLite over other databases**: SQLite was chosen because it is lightweight, requires no external server, and is ideal for small projects.
- **Minimal UI**: The interface was kept simple to emphasize functionality and clarity over visual complexity.
- **Single-page layout**: All interactions occur on one page, reducing navigation complexity and improving usability.

These choices ensured that the project remained achievable within the available time while still meeting CS50x requirements.

## Challenges and Lessons Learned

One of the main challenges was configuring the development environment correctly, particularly setting up Python and Flask on Windows.
This required understanding how package management works and how to resolve common PATH-related issues.

Another challenge was ensuring correct database handling, especially committing changes and closing connections properly.
Through this project, I gained a better understanding of how web applications interact with databases
and how backend logic connects to frontend interfaces.

## Conclusion

This To-Do App successfully demonstrates fundamental web development concepts taught in CS50x, including backend programming,
database usage, and dynamic content rendering. While the project is intentionally simple, it reflects thoughtful design choices,
clean organization, and practical implementation of computer science principles.

This project represents an important milestone in my learning journey and serves as a foundation for building more complex applications in the future.
