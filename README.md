# EJB Demo

## Build and Run with Docker

1.  **Package the application:**
    ```bash
    mvn package
    ```

2.  **Build the Docker image:**
    ```bash
    docker build -t ejb-demo -f Dockerfile2 .
    ```

3.  **Run the Docker container:**
    ```bash
    docker run -p 8080:8080 ejb-demo
    ```

4.  **Access the EJB via the Servlet:**
    Open your browser to [http://localhost:8080/ejb-demo-1.0-SNAPSHOT/hello-servlet](http://localhost:8080/ejb-demo-1.0-SNAPSHOT/hello-servlet)
    or use curl:
    ```bash
    curl http://localhost:8080/ejb-demo-1.0-SNAPSHOT/hello-servlet
    ```