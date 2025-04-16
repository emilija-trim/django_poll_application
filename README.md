# Polls App

This is a Django application for creating and managing polls. Users can create questions and multiple choices for each question, and they can vote on the choices.

## Project Structure

```
polls-app
├── polls
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── migrations
│   │   └── __init__.py
│   ├── models.py
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── manage.py
├── requirements.txt
└── README.md
```

## Requirements

```
    "django>=5.2",
    "django-debug-toolbar>=5.1.0",
```

## Features

- **Admin Interface**: Custom admin interface for managing questions and choices.
- **Model Definitions**: `Question` and `Choice` models to represent poll questions and their respective choices.
- **Recent Publication Check**: Functionality to check if a question was published recently.

## Installation

This project uses uv: https://docs.astral.sh/uv/

1. Initiate project:
   ```
   uv init
   ```
2. Copy and paste dependencies to pyproject.toml.

3. Install the required packages:
   ```
   uv sync
   ```

## Usage

To run the development server, use the following command:
```
uv run manage.py runserver
```

Visit `http://127.0.0.1:8000/` in your web browser to access the application.

## Testing

To run tests for the application, use:
```
uv run manage.py test
```
