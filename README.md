# Prisma x Python

Testing the functionality of Prisma with Python.

0. fill out the `.env` file with your credentials


1. start the docker container

```bash
docker-compose up -d
```

2. Generating Prisma Client Python

```bash
poetry run prisma db push
```

To change the schema use the migration as follows:

```bash
# apply migrations
poetry run prisma migrate dev --name "add comment model"
# generate
poetry run prisma generate
```