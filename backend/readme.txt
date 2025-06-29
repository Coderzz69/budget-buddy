budget-buddy/
├── backend/                       # Backend source code
│   ├── manage.py                  # Django CLI entry point
│   ├── .env                       # Environment variables
│   ├── requirements.txt           # Python dependencies
│   ├── src/                       # All source code
│   │   ├── controllers/           # Logic for handling requests
│   │   │   ├── auth_controller.py
│   │   │   ├── expense_controller.py
│   │   │   ├── budget_controller.py
│   │   ├── lib/                   # Helper libraries or services
│   │   │   ├── db.py              # DynamoDB setup and utilities
│   │   │   ├── utils.py           # Miscellaneous utilities
│   │   ├── middleware/            # Middleware logic
│   │   │   ├── auth_middleware.py # JWT verification
│   │   ├── models/                # Data models for DynamoDB
│   │   │   ├── user_model.py
│   │   │   ├── expense_model.py
│   │   │   ├── budget_model.py
│   │   ├── routes/                # URL routing
│   │   │   ├── auth_routes.py
│   │   │   ├── expense_routes.py
│   │   │   ├── index.py
│   │   ├── settings/              # Django settings split into environments
│   │   │   ├── base.py
│   │   │   ├── dev.py
│   │   │   ├── prod.py
│   │   ├── tests/                 # Unit and integration tests
│   │   │   ├── test_controllers/
│   │   │   │   ├── test_auth_controller.py
│   │   │   │   ├── test_expense_controller.py
│   │   │   ├── test_models/
│   │   │   │   ├── test_user_model.py
│   │   │   │   ├── test_expense_model.py
│   │   │   ├── test_routes/
│   │   │       ├── test_auth_routes.py
│   │   ├── wsgi.py                # For WSGI deployment
│   │   ├── asgi.py                # For ASGI deployment
│   │   ├── urls.py                # Main URL routing
│   │   ├── settings.py            # Main Django settings (entry point)
