# Django Blog Project

A simple blog application built using Django, where users can create, edit, and delete posts. It includes user authentication, comment functionality, and a clean user interface.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)

## Project Overview
This Django Blog Project allows users to:
- Create and manage blog posts.
- Add comments to posts.
- Edit or delete their own posts.
- View a list of all posts or filter posts by specific users.
- Basic user authentication (sign up, login, logout).

## Features
- User authentication (registration, login, logout).
- Blog post management (create, edit, delete).
- Commenting system for posts.
- Admin panel for managing content.

## Technologies Used
- **Django**: Web framework for building the blog.
- **SQLite**: Default database for development (you can switch to PostgreSQL or MySQL for production).
- **Bootstrap**: Frontend framework for styling and responsive design.
- **Python-decouple**: For managing environment variables.
- **Pillow**: For handling images in blog posts (if needed).

## Installation

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Django 3.2+
- Git

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/django-blog.git
   cd django-blog
   ```

2. **Set up a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**
   Create a `.env` file in the root directory and add the following (customize as needed):

   ```bash
   SECRET_KEY=your-secret-key
   DEBUG=True
   ALLOWED_HOSTS=localhost,127.0.0.1
   ```

5. **Apply the database migrations:**
   ```bash
   python manage.py migrate
   ```

6. **Create a superuser for the admin panel:**
   ```bash
   python manage.py createsuperuser
   ```

7. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

8. **Access the app:**
   Open your browser and go to `http://127.0.0.1:8000`.

## Environment Variables

Make sure you configure the following in your `.env` file:

```bash
SECRET_KEY=your-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
```

Additional configurations can be added depending on your setup (e.g., database credentials).

## Usage
Once you’ve started the server:
- Go to `http://127.0.0.1:8000` to view the blog.
- Create a new user or log in to manage posts.
- Use the Django admin panel at `http://127.0.0.1:8000/admin` to manage posts and users.
