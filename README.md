# data-academy
Repository to learn stuff about data

👏 **Shout out** to https://github.com/tiangolo/full-stack-fastapi-postgresql 

# requirements
1. Install docker
2. Install docker-compose

# setup
## data-academy-app
This will spin up all the services required to run:
1. Postgres DB (including PGAdmin)
2. FastAPI back-end (including Jupyter Notebook)
3. Swagger UI for API
4. Front-end for app user management
5. Celery for task management

In the same tab terminal:
- `cd data-academy-app`
- `docker-compose up`

## sql - jupyter notebook

Open another terminal:
- `cd data-academy-app`
- `docker-compose exec backend bash`
- `$JUPYTER`
