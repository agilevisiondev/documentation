# Documentation

build latest image for a service 
`sudo docker compose build --no-cache  api`

start only one specific container `sudo docker compose up -d api`

run db migration on prod `sudo npx dotenv -e .env.staging -- prisma migrate deploy`
make sure .env.staging has DB_URL and the database is running on `localhost:PORT` instead of `docker_container:PORT`
