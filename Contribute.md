## Docker Installation
- Install Docker
- Create a network - docker network create user_projects
- Start postgres
    - docker run --network user_projects --name postgres -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
- Build th image - `docker build --network=host -t user-project .`
- Start the imag - `docker run -e DATABASE_URL=postgresql://postgres:mysecretpassword@postgres:5432/postgres --network user_projects -p 3000:3000 user-project`

## Docker Compose installation steps
- Install docker, docker-compose
- Run `docker-compose up`