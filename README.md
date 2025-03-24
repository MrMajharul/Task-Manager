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
