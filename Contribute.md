## Docker Installation
- Install Docker
- Start postgres
    - docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
- Build th image - `docker build -t user-project .`
- Start the imag - `docker run -p 3000:3000 user-project`

## Docker Compose installation steps
- Install docker, docker-compose
- Run `docker-compose up`