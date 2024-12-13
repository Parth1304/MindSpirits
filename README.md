# MindSpirits - Django Chat Room Application

A Django-based web application that allows users to create rooms, send messages, and interact in a chat environment. This project includes features like user authentication (login, registration), user profiles, activity feed, and CRUD operations for messages. The project also integrates with the Django REST Framework for future API development.

## Features

- **User Authentication**: Login, registration, and logout functionality with Flash Messages.
- **Chat Room**: Users can create, join, and participate in chat rooms.
- **CRUD Operations**: Create, read, update, and delete messages in chat rooms.
- **User Profiles**: Each user has a personalized profile page displaying their activities.
- **Activity Feed**: A feed displaying recent activities (messages) in the system.
- **Search**: Search functionality for rooms and messages.
- **Responsive Design**: Mobile-friendly UI using CSS and Bootstrap.
- **Django Admin Panel**: Easy management of rooms, messages, and users.

## Prerequisites

To run this project locally, you need to have the following installed:

- Python 3.8+
- pip (Python package installer)
- Django 4.2.3 (or later)
- PostgreSQL (or another database of your choice)
- Optional: Docker (for containerized environment)

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/mindspirits.git
    cd mindspirits
    ```

2. **Set up a virtual environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # For Linux/MacOS
    .\venv\Scripts\activate  # For Windows
    ```

3. **Install the dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Setup the database**:
    - Make sure your database (e.g., PostgreSQL) is set up and configured in the `settings.py` file under `DATABASES`.
    - Run migrations:
      ```bash
      python manage.py migrate
      ```

5. **Create a superuser (for accessing the Django admin)**:
    ```bash
    python manage.py createsuperuser
    ```

6. **Run the development server**:
    ```bash
    python manage.py runserver
    ```
    Now you can visit the app at `http://127.0.0.1:8000/`.

## Usage

1. Visit the home page and either log in or register as a new user.
2. After logging in, you can:
    - Create and join chat rooms.
    - Send and receive messages in rooms.
    - View and edit your profile.
    - Use the search functionality to find specific rooms or messages.
3. The admin panel can be accessed at `http://127.0.0.1:8000/admin` (use the superuser credentials).

## Files and Directories

- **`manage.py`**: The main entry point for running Django commands.
- **`mindspirits/`**: The main project directory containing settings and app configurations.
- **`base/`**: The app for handling user authentication, rooms, and messages.
- **`templates/`**: HTML templates for the frontend pages.
- **`static/`**: Static files (CSS, JS, images) for the frontend.
- **`requirements.txt`**: Lists the project dependencies.

## Contributing

1. Fork this repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push them to your fork.
4. Open a pull request to the main repository.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Django Framework
- Bootstrap for responsive design
- PostgreSQL for database management
- Inspiration from various Django tutorials

---

Feel free to adjust the above template according to your project details.
