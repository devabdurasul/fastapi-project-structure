# FastAPI Folder Structure

This repository provides a clean and modular folder structure template for building FastAPI applications. It’s organized to help developers quickly set up, understand, and expand a FastAPI-based project. Ideal for scalable APIs with features such as database management, authentication, and organized routes.


## 📁 Project Structure Overview

fastapi_folder_structure/
├── app/
│   ├── __init__.py
│   ├── main.py            # Entry point of the application
│   ├── core/
│   │   ├── __init__.py
│   │   ├── config.py       # Configuration and settings
│   │   └── security.py     # Authentication and security functions
│   ├── api/
│   │   ├── __init__.py
│   │   ├── api_v1/
│   │   │   ├── __init__.py
│   │   │   ├── endpoints/
│   │   │   │   ├── __init__.py
│   │   │   │   └── items.py
│   │   │   └── router.py
│   ├── models/
│   │   ├── __init__.py
│   │   └── item.py
│   ├── schemas/
│   │   ├── __init__.py
│   │   └── item.py
│   ├── crud/
│   │   ├── __init__.py
│   │   └── item.py
│   ├── db/
│   │   ├── __init__.py
│   │   ├── base.py
│   │   └── session.py
│   ├── tests/
│   │   ├── __init__.py
│   │   └── test_items.py
│   └── utils/
│       ├── __init__.py
│       └── helpers.py
├── .env
├── .gitignore
├── requirements.txt
├── README.md
└── alembic/

### Folder Details

* app/main.py: The main entry point. Initializes the FastAPI instance, includes routers, and configures middleware.
* app/core/: Contains configuration (config.py) and security (security.py) settings.
* app/api/: Organized API versions (api_v1) with modular endpoint files.
* app/models/: SQLAlchemy models defining database schemas.
* app/schemas/: Pydantic schemas for request validation.
* app/crud/: CRUD logic for database operations.
* app/db/: Database session and metadata configuration.
* app/tests/: Test suite for unit and integration tests using pytest.
* app/utils/: Helper functions used across the project.


## 🚀 Getting Started

**Clone the repository**

git clone https://github.com/yourusername/fastapi_folder_structure.git
cd fastapi_folder_structure


## 🔧 Key Features

* Modular structure for scalable FastAPI applications
* Database handling with SQLAlchemy
* Easy-to-use environment-based configurations
* Basic CRUD operations and example endpoints
* Built-in authentication and security stubs
* Interactive API documentation


## 📝 License

This repository is open-sourced and available under the MIT License.

--------------------------------------------------------------------------------------------------------------------------

Feel free to customize this to better reflect any unique aspects of your setup!