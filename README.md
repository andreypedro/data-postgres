# data-postgres

´´´Docker command
sudo dockerd
docker pull postgres

# creating a container
docker run --name data-engineering-postgres -e POSTGRES_PASSWORD=secret -d postgres

# creating a database
docker exec -u postgres data-engineering-postgres createdb postgres-db

# entrying in container
docker exec -it data-engineering-postgres psql -U postgres -d postgres-db

# creating a table
Importing data:
https://transparent-trout-f2f.notion.site/SQL-7bc979523659472d8c2b6e36e64ff113

# Seeing the tables
\dt
´´´