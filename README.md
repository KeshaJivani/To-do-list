# To-Do List App

## Overview
This is a simple Android To-Do List application that allows users to add, delete, and update tasks. It utilizes SQLite for data persistence and follows an MVC structure.

## Features
- Add tasks to the list
- Delete tasks by clicking on them
- Persistent storage using SQLite
- Simple UI with EditText, Button, and ListView

## Project Structure
```
/app/src/main/java/com/example/to_do_list/
│-- MainActivity.java
│-- DatabaseHelper.java
│
/app/src/main/res/layout/
│-- activity_main.xml
│
```

## Files & Explanation

### MainActivity.java
Handles user interaction, updates UI, and communicates with `DatabaseHelper` for data persistence.

### activity_main.xml
Defines the UI layout, including an EditText for task input, a Button to add tasks, and a ListView to display tasks.

### DatabaseHelper.java
Manages SQLite database operations such as adding, retrieving, updating, and deleting tasks.

## Setup & Installation
1. Clone or download the repository.
2. Open the project in **Android Studio**.
3. Sync Gradle and build the project.
4. Run the app on an emulator or a real device.

## Usage
- Enter a task in the input field and click **Add Task**.
- Click on a task in the list to **delete it**.

## Database Schema
**Table Name:** `tasks`
| Column      | Type          | Description             |
|------------|--------------|-------------------------|
| id         | INTEGER (PK)  | Auto-increment ID      |
| task       | TEXT          | Task description       |
| timestamp  | TIMESTAMP     | Default: current time  |

## License
This project is open-source and available under the **MIT License**.

