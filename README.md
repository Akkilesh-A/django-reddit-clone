# 🛠️ Reddit Clone Backend

A simple backend implementation for a Reddit-like application built with Django and Django REST Framework (DRF).

## ✨ Features

- **Posts**:
    - 📝 Create new posts.
    - ❌ Delete existing posts.
- **Voting**:
    - 👍 Upvote posts.
    - 🗑️ Remove votes from posts.

## 🖥️ Tech Stack

- **Backend Framework**: [Django](https://www.djangoproject.com/)
- **API Framework**: [Django REST Framework (DRF)](https://www.django-rest-framework.org/)

## 🚀 Installation

1. Clone the repository:
    
    ```bash
    git clone https://github.com/Akkilesh-A/django-reddit-clone
    cd django-reddit-clone
    
    ```
    
2. Create and activate a virtual environment:
    
    ```bash
    python -m venv reddit-clone-venv
    reddit-clone-venv\Scripts\activate
    
    ```
    
3. Install the dependencies:
    
    ```bash
    pip install -r requirements.txt
    
    ```
    
4. Apply database migrations:
    
    ```bash
    python manage.py migrate
    
    ```
    
5. Run the development server:
    
    ```bash
    python manage.py runserver
    
    ```
    

## 🔗 API Endpoints

### 🔐 Authentication

- `GET /api-auth/login/` - Log in (DRF's default authentication interface).
- `GET /api-auth/logout/` - Log out (DRF's default authentication interface).

### 📝 Posts

- `GET /api/posts` - Retrieve a list of posts.
- `POST /api/posts` - Create a new post.
- `GET /api/posts/<int:pk>` - Retrieve a specific post.
- `DELETE /api/posts/<int:pk>` - Delete a specific post.

### 👍 Votes

- `POST /api/posts/<int:pk>/vote` - Create a vote for a specific post.

## 🗂️ Project Structure

```
reddit-clone/
│
├── posts/                # Django app for managing posts
├── reddit_clone/         # Main Django project configuration
├── .gitignore            # Git ignore file to exclude unnecessary files
├── manage.py             # Django's management script
├── requirements.txt      # File listing project dependencies
```
