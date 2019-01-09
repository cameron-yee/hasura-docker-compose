# hasura-docker-compose

## Usage

1. Set Environment variables for PostgreSQL image and Hasura image in .env in project root folder
    * Hasura Environment Variables: HASURA_GRAPHQL_DATABASE_URL, HASURA_GRAPHQL_ENABLE_CONSOLE

    <a href="https://docs.hasura.io/1.0/graphql/manual/deployment/docker/index.html" target="_blank">See Docs</a>

    * Postgres Environment Variables: POSTGRES_PASSWORD, POSTGRES_USER, POSTGRES_DB

    * When setting the db connection string in the HASURA_GRAPHQL_DATABASE_URL, use the postgres container name as the hostname

2. Run: docker-compose -f .docker/dev/dev.docker-compose.yml up -d
3. Go to Hasura console at localhost:8080
