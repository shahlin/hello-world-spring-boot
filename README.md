# Hello World Spring Boot API

## Setup
1. Make sure Docker engine is running
2. Build the docker image using the command:
    ```bash
    $ docker build -t spring-boot-docker:spring-docker .
    ```
3. Run the container:
    ```
    $ docker run -p 8080:8080 spring-boot-docker:spring-docker .
    ```
4. Test by visiting the endpoint: `http://localhost:8080/`

## Changing API Version
1. Open `pom.xml`
2. Update the `version` element under `project` 

## API Endpoints
1. Root - `GET` /
2. Greet - `GET` /greet/{name}
3. Health Check - `GET` /health/ready
4. Version Check - `GET` /version