
# Task Manager

## Description

**Task Manager** is a web application built with **Django** that helps users organize and manage their tasks. It provides features like task creation, updates, deletion, and more. The app integrates **Celery** for background task processing and uses **Django Channels** for real-time updates. It also allows users to export task data in various formats like CSV, Excel, and PDF.

This project is ideal for individuals or teams looking for an organized, interactive, and real-time task management solution.

## Features

- **User Authentication:** Users can sign up, log in, and manage their accounts.
- **Task Management:** Create, edit, delete, and track tasks.
- **Real-Time Updates:** Tasks are updated in real-time using Django Channels.
- **Background Task Processing:** Asynchronous task processing using Celery.
- **Data Export:** Export tasks to CSV, Excel, or PDF formats.

## Technologies Used

- **Django** - Web framework
- **Celery** - Asynchronous task queue
- **Redis** - Message broker for Celery
- **Django Channels** - Real-time WebSocket support
- **PostgreSQL** - Database management
- **Bootstrap** - Frontend styling (for the UI)
- **Python 3** - Programming language

## Installation

Follow these steps to run the project locally:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/task_manager.git
   cd task_manager
   ```

2. **Set up a virtual environment:**
   Create a virtual environment:
   ```bash
   python3 -m venv venv
   ```

   Activate the virtual environment:

   **On macOS/Linux:**
   ```bash
   source venv/bin/activate
   ```

   **On Windows:**
   ```bash
   venv\Scriptsctivate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure the database:**
   Run the migrations to set up the database schema:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create a superuser to access the Django admin:**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run the development server:**
   ```bash
   python manage.py runserver
   ```

7. **Start Celery Worker for background tasks:**
   ```bash
   celery -A task_manager worker --loglevel=info
   ```

8. **Visit the application:**
   Open your browser and navigate to:
   ```bash
   http://127.0.0.1:8000
   ```

## Deployment

You can deploy the Task Manager app using Railway. Follow these steps to deploy:

1. **Install the Railway CLI:**
   ```bash
   npm install -g railway
   ```

2. **Log in to your Railway account:**
   ```bash
   railway login
   ```

3. **Link the project to Railway:**
   ```bash
   railway link
   ```

4. **Deploy the project:**
   ```bash
   railway up
   ```

5. **Access the live application** through the provided Railway link.

## Contributing

We welcome contributions to this project. To contribute:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Commit your changes:
   ```bash
   git commit -am 'Add new feature'
   ```
4. Push your changes to your fork:
   ```bash
   git push origin feature-branch
   ```
5. Open a pull request to the main repository.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements

- **Django**: The primary web framework used.
- **Celery**: For background task processing.
- **Redis**: As a message broker for Celery.
- **Django Channels**: For real-time functionality in the app.
- **Bootstrap**: For UI styling.
