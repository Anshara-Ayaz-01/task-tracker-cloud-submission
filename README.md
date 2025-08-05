# Project Overview
Task Tracker Lite is a full-stack MERN application for managing tasks with features like user authentication, task CRUD operations, overdue detection, and pagination.
This version is cloud-deployed, with:

->Backend hosted on Render
->Frontend hosted on Vercel

------------Frontend (Vercel):----------------------------
-[Open Frontend on Vercel](https://task-tracker-frontend-f6aksx19j-anshara-ayazs-projects.vercel.app/)

------------Backend (Render):------------------------------
-[Ope Backnd on Render](https://task-tracker-backend-462y.onrender.com/)

**Features**

Backend (Node.js + Express + MongoDB)

User Authentication (Signup/Login/Logout)

Task CRUD (Create, Read, Update, Delete)

Overdue task detection

JWT token + HttpOnly Cookie Authentication

Error handling and clean code

**Frontend (React)**

Signup and Login pages

Task dashboard with:

Add new task

View all/overdue tasks

Pagination

Mark task as completed

Logout functionality

 **Logical Flow**

Authentication Flow-------------------------------

User signs up → Data saved to MongoDB (via backend API).

On login → JWT is issued & stored in HttpOnly cookie.

Authenticated requests automatically include the cookie for task access.

**Task Management Flow**

On dashboard load → /api/tasks is called with credentials.

User can:

Add a new task (POST /api/tasks)

View overdue tasks (GET /api/tasks/overdue)

Mark task copleted (PATCH /api/tasks/:id)

Tasks are paginated on frontend using state-based slicing.

styled UI


**For Login signup new user or enter existing users that is already in database**

email:anu@example.com
password:anu123

email:liza@example.com
password:liza123

email:xyz@example.com
password:xyz123



