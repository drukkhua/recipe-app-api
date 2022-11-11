# recipe-app-api
Recipe API project
- TDD (GitHub Actions test all project when get new Push request)
- RestAPI with custom serializers
- Wait_for_db - DB run first & all commands run after run DB
- Rest_framework.authtoken -> authentication with token
- Documentation for API - > drf_spectacular
- Flake8
- Docker compose for PostgreSQL & all project
---
- First run project:
<br>- <code>docker-compose build .</code>
<br>- <code>docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate</code>
---
- To run all 62 tests & flake8 test local:
<br> -<code>docker-compose run app sh -c "python3 manage.py test && flake8"
</code>
---
- Run project after locally: 
<br>- <code>docker-compose up</code>