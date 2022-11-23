# django-tdd-docker
# Docker and App
  ```
  docker build .
  docker-compose build
  docker-compose run app sh -c "django-admin startproject app ."
  cd app
  docker-compose run app sh -c "python manage.py startapp api"
  ```
# Docker interactive shell

```
  docker-compose up -dd
   docker-compose exec app /bin/sh
```

# Testing setup
- Create folder "tests" in app. Delete existing tests.py
- Create __init__.py in tests folder
- Create different test files for different purposes starting with "test_"
- Each file contains a class that contains different unit tests as methods named "test_<functionality_name>()"


# Creating model test
- Create Tests
  -- Fails: Model not found
- Code Model
  - Fails: Model not registered in installed apps
- Add API to Installed Apps
  - Fails: Table not found
- Make migrations and migrate


