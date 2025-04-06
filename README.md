# assignment1

Web Application Mini Projects - JavaScript Practical

This project includes three interactive web-based mini applications built using **HTML**, **CSS**, and **Vanilla JavaScript**:

1. **Weather Forecast Tracker**
2. **Task Management System**
3. **Online Shopping Cart**

Each mini project demonstrates core JavaScript concepts like array manipulation, DOM updates, event handling, filtering, sorting, and conditional rendering.

---

## 1️⃣ Weather Forecast Tracker

### Description
This app displays weather information for a list of cities and provides interactive features like:
- Add new city with random weather
- Remove cities
- Sort cities by temperature (hottest first)
- Filter cities by weather condition (Sunny / Rainy)

### Features
- Uses JavaScript array methods like `.push()`, `.filter()`, `.sort()`
- Dynamically renders list using `.map()`
- Event-driven UI interactions
- Clean and responsive CSS UI

---

## 2️⃣ Task Management System

### Description
A simple task manager to keep track of tasks with priority and completion status.

### Features
- Add new task with random priority
- Mark task as completed
- Filter tasks by status: Pending / Completed
- Sort tasks by priority (ascending)
- Styled to distinguish between completed and pending tasks

---

## 3️⃣ Online Shopping Cart

### Description
A functional shopping cart that simulates product addition, removal, and price calculation.

### Features
- Add new random product with a price
- Remove product from the cart
- Calculate total cart value using `.reduce()`
- Dynamic UI updates using DOM methods
- Uses `toFixed()` for price formatting

---

## 🔧 How to Run

1. Clone or download this repository.
2. Open each HTML file (for each mini project) in a modern web browser.
3. Interact with the buttons to perform actions on each interface.

---

## 💡 Learning Objectives

- DOM Manipulation using JavaScript
- Working with arrays and JavaScript objects
- Event handling in web apps
- Basic UI/UX styling with CSS
- Functional programming concepts in JS (map, filter, reduce, sort)

---

## 📂 Files

- `weather.html`
- `card.html`
- `index.html`

---

# assignment 2

Mini Web Projects 🚀

This repository contains three simple yet functional web-based applications built using **HTML**, **CSS**, and **JavaScript**. These projects are perfect for beginners to understand basic DOM manipulation, event handling, and time-based functionality in JavaScript.

## 🌟 Projects Included:

1. [✅ **Online Appointment Scheduler**](#1-online-appointment-scheduler)
2. [💰 **Expense Tracker**](#2-expense-tracker)
3. [📚 **Study Planner**](#3-study-planner)

---

## 1. ✅ Online Appointment Scheduler

### 🔹 Features:
- Add client appointments with time and service type
- View appointments scheduled within the next hour
- Automatically logs a reminder to the console before the appointment

### 🔹 Technologies:
- HTML5
- CSS3
- JavaScript

### 🔹 How It Works:
- Takes client name, time, and service type.
- Checks if the appointment is within the next hour and displays it in the “Upcoming Appointments” section.
- Uses `setTimeout()` to simulate a reminder message.

---

## 2. 💰 Expense Tracker

### 🔹 Features:
- Add expenses with description, amount, and date
- Calculates total expenses
- Filter expenses between two dates
- Simulates fetching expense report with a `Promise`

### 🔹 Technologies:
- HTML5
- CSS3
- JavaScript

### 🔹 How It Works:
- Inputs are validated for correctness.
- Total is dynamically updated.
- Filters list based on selected date range.

---

## 3. 📚 Study Planner

### 🔹 Features:
- Add a study session with topic, time, and duration
- View today's sessions
- View all added sessions

### 🔹 Technologies:
- HTML5
- CSS3
- JavaScript

### 🔹 How It Works:
- Sessions are stored in memory.
- Displays only today’s sessions in one section and all sessions in another.
- Good for managing daily study routines.

---

## 🛠 How to Run

1. Clone or download this repository.
2. Open each `.html` file in your browser:
   - `appointment_scheduler.html`
   - `expense_tracker.html`
   - `study_planner.html`
3. All projects run independently and require no additional setup.

---
## 💡 Future Improvements
- Store data using `localStorage` to persist sessions/appointments/expenses
- Add edit/delete functionality
- Responsive design improvements
- Option to export reports

---

# assignment 3
# 🔧 Node.js Command-Line Utilities

This project contains **three mini command-line tools** built using Node.js:

1. 📁 **File Organizer**
2. 💾 **File Backup System**
3. 🧠 **Environment Inspector**

Each tool solves a specific filesystem or environment-related problem and runs from the terminal.

---

## 1. 📁 File Organizer

### 🎯 Objective
Automatically organize files in a given directory into categorized subfolders based on file types (Images, Documents, Videos, Others).

### ✅ Features
- Scans a target directory
- Detects common file types by extension
- Creates folders like `Images/`, `Documents/`, etc.
- Moves files into the correct subfolder
- Uses `fs` and `path` modules
- Includes error handling using `try...catch`


### 🚀 Usage

```bash
node organizer.js <target-folder-path>
```

## 2.💾 File Backup System 

### 🎯 Objective
Back up files from a given folder to a backup/ folder, maintaining original structure and optionally compressing into a .zip.
### ✅ Features
- Recursively copies all files/folders into backup/
- Maintains the original folder structure using path
- Logs all file names, sizes, and timestamps to backup-log.txt
- Optional: Compress backup folder using --zip flag
- Uses fs, path, archiver
- Handles file permission and missing file errors


### 🚀 Usage

```bash
node backup.js <source-folder-path> [--zip]
```


## 3. 🧠 Environment Inspector

### 🎯 Objective
Inspect and save the current system’s environment details like hostname, home directory, interfaces, and environment variables.


### ✅ Features
- Uses os module to display:
   - Home directory
   - Hostname
   - Network interfaces
- Uses process.env to get environment variables
- Writes data to logs/env-details.json
- Gracefully handles file system errors

### 🚀 Usage

```bash
node env-inspector.js

```

# assignment4

📦 Order Management System

A secure and role-based Order Management System API built using **Node.js**, **Express**, **MongoDB**, and **JWT**. This system allows authenticated users to manage orders and includes features such as authentication, logging, centralized error handling, and role-based access control.

---

## 🚀 Features

- ✅ CRUD operations for managing orders
- 🔐 JWT-based user authentication
- 🍪 HTTP-only cookie session management
- 🧾 Request logging to `server.log`
- ⚠️ Centralized error handling
- 🛡️ Role-based access control (Admin/User)
- 💾 MongoDB for database storage

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **MongoDB** with **Mongoose**
- **JWT** for Authentication
- **bcryptjs** for Password Hashing
- **cookie-parser** for Cookie Management
- **dotenv** for Environment Variables
- **fs** for Logging Middleware

---

## 📁 Project Structure
order-management/ │ ├── controllers/ │ ├── authController.js │ └── orderController.js │ ├── middleware/ │ ├── auth.js │ ├── errorHandler.js │ ├── logger.js │ └── roleCheck.js │ ├── models/ │ ├── Order.js │ └── User.js │ ├── routes/ │ ├── authRoutes.js │ └── orderRoutes.js │ ├── server.js ├── server.log ├── .env └── package.json




# assignment5
# 📝 Blog Application API

A RESTful API built using **Express** and **MongoDB (Mongoose)** that allows you to manage blog posts and authors. Demonstrates modern best practices such as modular architecture, Mongoose relationships (`ref` and `populate`), data validation, and robust error handling.

---

## 📦 Tech Stack

- **Node.js**
- **Express**
- **MongoDB**
- **Mongoose**
- **dotenv**

---

## 🚀 Features

✅ Create and manage authors  
✅ Create blog posts linked to authors  
✅ Fetch blog posts with author details (`populate`)  
✅ Validate input using Mongoose validation  
✅ Clean modular architecture (models, routes, controllers)  
✅ Error handling middleware for consistent responses

---

## 🛠️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/vaghasiyaMira07/fswd-assignments
```

📂 Project Structure
blog-api/
├── models/
│   ├── Author.js
│   └── BlogPost.js
├── controllers/
│   ├── authorController.js
│   └── blogPostController.js
├── routes/
│   ├── authorRoutes.js
│   └── blogPostRoutes.js
├── app.js
├── .env
└── package.json


# assignment6
# 🛍️ Responsive Product Card (React + CSS Modules)

A simple and stylish **responsive product card** built using **React** and **CSS Modules**. This project demonstrates how to apply modern styling techniques, including scoped CSS and responsive design principles in a React application.
---

## 🚀 Features

- 🎨 Styled with **CSS Modules** for component-level scoping
- 📱 Fully **responsive layout** for all screen sizes
- 🔄 Smooth **hover effects**
- 💡 Clear example of passing props (`name`, `price`, `description`) into components

---

## 📂 Project Structure

esponsive-product-card/ ├── src/ │ ├── components/ │ │ └── ProductCard.js │ │ └── ProductCard.module.css │ ├── App.js │ └── index.js ├── package.json └── README.md
