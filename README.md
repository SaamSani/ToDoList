# ToDoList

A simple To-Do List application built with Node.js, Express, PostgreSQL, and EJS templates. The app allows users to manage tasks with features such as adding, editing, and deleting items. The tasks are stored in a PostgreSQL database for persistence.

## Features

- Add new tasks
- Edit existing tasks
- Delete tasks by checking them off
- Store tasks in a PostgreSQL database
- Responsive user interface built with EJS and custom CSS

## Technologies Used

- **Node.js**: JavaScript runtime environment
- **Express**: Web framework for Node.js
- **PostgreSQL**: Relational database for storing tasks
- **EJS**: Template engine for rendering views
- **CSS**: For styling the user interface

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/SaamSani/ToDoList.git
   cd ToDoList
2. Install dependencies:
   
   ```bash
   npm install
3. Ensure PostgreSQL is installed on your machine. You can download and install it from here.
   Create a new database called permalist. You can do this by logging into the PostgreSQL terminal and running:

   ```bash
   CREATE DATABASE permalist;
4. Create the items table inside the permalist database by running the following SQL command:

   ```bash
   CREATE TABLE items (
   id SERIAL PRIMARY KEY,
   title VARCHAR(255)
   );
5. Update the db connection settings in index.js,
   Inside your solution.js file, update the database connection settings with your PostgreSQL credentials as shown below:

   ```bash
   const db = new pg.Client({
   user: "your-username",   // replace with your PostgreSQL username
   host: "localhost",
   database: "permalist",   // the database name you created
   password: "your-password",   // your PostgreSQL password
   port: 5432,
   });
6. Run:

   ```bash
   nodemon index.js
7. Open your browser and navigate to:

   ```bash
   http://localhost:3000




   

   


   


