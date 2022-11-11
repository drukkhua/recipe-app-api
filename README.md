# recipe-app-api
Recipe API project
- TDD (GitHub Actions test all project when get new Push request)
- RestAPI with custom serializers
- wait_for_db
- rest_framework.authtoken -> authentication with token
- drf_spectacular -> for documentation API
- Flake8
- docker compose for PostgreSQL & all project
to run all 62 tests & flake8 test type command: docker-compose run app sh -c "python3 manage.py test && flake8"
first run project: docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate
