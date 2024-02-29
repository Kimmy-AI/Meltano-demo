## Meltano-demo
An ELT pipeline

# Configuaration
Set environment variables:  
Create a new ".env" file following the example shown in ".env.example" and enter your own environment variables.  
The project requires the following environment variables to be input:
```env
TAP_GITHUB_AUTH_TOKEN=
TARGET_POSTGRES_PASSWORD=
DBT_POSTGRES_PASSWORD=
```

# Step 1 - run your EL pipeline
> `meltano run tap-github target-postgres`

You can do your first complete EL run by calling `meltano run`!

# Step 2 - view database in docker
> `docker run --name meltano_postgres -e POSTGRES_PASSWORD=password -p 5432:5432 -d postgres`

if docker is running on port 5432, excute command below

> `docker exec -it meltano_postgres bash`

> `psql -U meltano -d postgres`