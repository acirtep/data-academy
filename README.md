# data-academy
Repository to learn stuff about data

👏 **Shout out** to https://github.com/tiangolo/full-stack-fastapi-postgresql 

# requirements
1. Install docker
2. Install docker-compose

# setup
## data-academy-app
This will spin up all the services required to run:

1. Postgres DB (including PGAdmin) @ localhost:5050

2. FastAPI back-end (including Jupyter Notebook) 

3. Swagger UI for API @ localhost:80/docs

4. Front-end for app user management @ localhost:80

5. Celery for task management with flower @ localhost:5555

6. Traefik for traffic monitoring @ localhost:8090

In the same tab terminal:
- `cd data-academy-app`
- `docker-compose up`

## how to install new python dependencies
Open another terminal:
- `cd data-academy-app`
- `docker-compose exec backend bash`
- `poetry add ` python_dependency

## sql - jupyter notebook

Open another terminal:
- `cd data-academy-app`
- `docker-compose exec backend bash`
- `$JUPYTER`
- open the Jupyter link and check the SQL_workbench notebook

## how to plot data on the world map (Jupyter Notebook)
- `cd data-academy-app`
- `docker-compose exec backend bash`
- `$JUPYTER`
- open the Jupyter link and check the how_to_draw_world_map notebook
- the html is available at /jupyter_notebooks

## how to plot data on the world map (Python)
- `cd data-academy-app`
- `docker-compose exec backend bash`
- `cd app`
- `python py_scripts/export_world_map.py `
- the html is available at /app/exports
