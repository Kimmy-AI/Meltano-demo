**Let's go ahead and build it ourselves within 5 minutes**

# Step 1 - run your EL pipeline
> `meltano run tap-github target-postgres`

You can do your first complete EL run by calling `meltano run`!

# Step 2 - view database in docker
> `docker run --name meltano_postgres -e POSTGRES_PASSWORD=password -p 5432:5432 -d postgres`

if docker is running on port 5432, excute command below

> `docker exec -it meltano_postgres bash`

> `psql -U meltano -d postgres`