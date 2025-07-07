Task Zen


Task Zen is a user-friendly task manager for organizing teams, projects, and tasks within a company. Managers can assign tasks, set deadlines, group tasks into projects, and manage team structures. Employees can upload work, submit for review, and get notified when tasks are reviewed.

🌟 Key Features
Dashboard:
View tasks overview (total, completed, pending, missed). Admins also see urgent/missed tasks and recent teams/projects.

Teams:
Organize and manage employees into teams. Admins can create/edit/delete teams.

Projects:
Available to Admins/Managers. Group tasks, track progress with a visual bar, and manage project data.

Tasks:
Create, assign, edit, and track tasks. Visibility settings control who can see what. Employees must upload files to submit tasks for review.

Reviews:
Admins/Managers review submitted tasks. Task status updates automatically when reviews are approved or rejected.

Mobile-Friendly:
Fully responsive design using Bootstrap 5 with custom styles.


⚙️ Tech Overview
Frontend: React (SPA) with react-router-dom

Backend: Django 5.0.3 (API-based), using class-based views and DRF serializers

Integration: Django serves the React build; django-cors-headers handles CORS; WhiteNoise serves static files

Database: 10 interconnected models with complex relationships

Extras: Pagination, filters, CSRF/session handling, seamless React-Django integration


👥 Roles & Usage
Register: Choose a role (Admin, Manager, Employee) and a company name (used to group users).

Admin/Manager: Full access to manage teams, projects, tasks, and reviews.

Employee: Assigned tasks, upload files, submit for review, view reviews and teams.

📁 File Structure Highlights
Backend (/task_manager/)

models.py: 10 core models (User, Task, Project, etc.)

views.py: API views and template rendering

serializers.py: DRF serializers for all models

Frontend (/react/)

components/: Reusable UI elements

routes/: Page-level logic

utils/: Helpers (auth, alerts, CSRF)

App.jsx: Route definitions

main.jsx: Entry point