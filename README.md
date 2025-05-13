# data-postgres

```bash
# Starting Docker daemon
sudo dockerd

# Pulling the PostgreSQL image
docker pull postgres

# Creating a container
docker run --name data-engineering-postgres -e POSTGRES_PASSWORD=secret -d postgres

# Creating a database
docker exec -u postgres data-engineering-postgres createdb postgres-db

# Entering the container
docker exec -it data-engineering-postgres psql -U postgres -d postgres-db

# Importing data
# Refer to the following link for SQL scripts and instructions:
# https://transparent-trout-f2f.notion.site/SQL-7bc979523659472d8c2b6e36e64ff113

# Viewing the tables
\dt