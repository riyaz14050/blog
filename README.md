# Django Blog Project

A simple Django blog application with authentication, CRUD functionality, and an admin interface.

## Overview
This application allows users to create, edit, and delete blog posts. Users can register and log in to manage their own posts, while an admin interface enables site management. The homepage displays all published posts, and users have access to a personalized dashboard to view their own posts.

## Setup Instructions

### 1. Clone Repository
```bash
git clone https://github.com/riyaz14050/blog.git
cd blog
```

### 2. Create and Activate Virtual Environment
```bash
python -m venv venv
# Windows: venv\Scripts\activate
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run Migrations
```bash
python manage.py makemigrations  # Create migration files
python manage.py migrate         # Apply database migrations
```

### 5. Create Admin User
```bash
python manage.py createsuperuser
```

### 6. Run Development Server
```bash
python manage.py runserver
```
Access the application at: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Features

- **User Authentication**: Sign up, login, and logout functionality
- **Blog Post Management**:
  - Create new blog posts (authenticated users)
  - Edit existing posts (post authors only)
  - Delete posts (post authors only)
  - View all posts on home page
- **My Posts Dashboard**: View and manage all your posts in one place
- **Admin Interface**: Full content management through Django admin panel
- **Security Features**:
  - CSRF protection
  - User authorization checks
  - Password hashing
- **Responsive Design**: Clean and simple user interface
