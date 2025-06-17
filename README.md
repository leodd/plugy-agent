# Plugy Agent API

A FastAPI-based backend application.

## Prerequisites

- Python 3.9 or higher
- Poetry (Python package manager)

## Setup

1. Install Poetry if you haven't already:
```bash
curl -sSL https://install.python-poetry.org | python3 -
```

2. Install dependencies:
```bash
poetry install
```

3. Activate the virtual environment:
```bash
poetry shell
```

## Running the Application

To run the development server:

```bash
uvicorn src.main:app --reload
```

The API will be available at `http://localhost:8000`

## API Documentation

Once the server is running, you can access:
- Swagger UI documentation: `http://localhost:8000/docs`
- ReDoc documentation: `http://localhost:8000/redoc`

## Development

- Format code:
```bash
poetry run black .
poetry run isort .
```

- Run tests:
```bash
poetry run pytest
```

## Project Structure

```
.
├── pyproject.toml      # Poetry configuration and dependencies
├── README.md          # This file
└── src/              # Source code
    └── main.py       # Main application file
``` 