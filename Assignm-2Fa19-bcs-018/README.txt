# Creation of MicroServices By utilizing Docker Compose

The undertaking involves the two microservices that operate as a server and client respectively. These microservices are launched through Docker Compose, a tool that facilitates the deployment of multiple services. When a request is submitted to the server, it computes the square root of an integer n and returns the result. Subsequently, the client makes a GET request to retrieve the outcome from the server, which is then displayed to the user.

## Folder Structure

The project folder structure should be organized as follows:

Assignment2/
|-- docker-compose.yml
|-- server/
| |-- Dockerfile
| |-- requirements.txt
| |-- app/
| | |-- server.py
|-- client/
| |-- Dockerfile
| |-- requirements.txt
| |-- app/
| | |-- client.py
|-- README.txt

- `docker-compose.yml`: Docker Compose file specifying the services to be built and run.
- `server/`: Folder containing the server microservice.
  - `Dockerfile`: Dockerfile specifying how the server container should be built.
  - `requirements.txt`: Requirements file specifying the Python dependencies for the server.
  - `app/`: Folder containing the server code.
    - `server.py`: Python script for the server.
- `client/`: Folder containing the client microservice.
  - `Dockerfile`: Dockerfile specifying how the client container should be built.
  - `requirements.txt`: Requirements file specifying the Python dependencies for the client.
  - `app/`: Folder containing the client code.
    - `client.py`: Python script for the client.
- `README.txt`: This readme file.

## Deployment

To deploy the microservices via Docker Compose, you need to follow these simple steps:

1. Verify that Docker and Docker Compose are already installed on your system.
2. Download and save a copy of this repository onto your local machine.
3. Navigate to the Assignment2 directory.
4. Type the command "docker-compose up" to build and execute the client and server containers.
5. Both client and server containers will be generated and executed successfully. The server will run on port 5000 while the client will obtain the square root of n by requesting the server.
6. The output retrieved from the server will be displayed by the client.
Important: Ensure that no other processes are currently operating on port 5000 as it is exclusively reserved for the server in this project.

And there you go! You have effectively deployed the microservices utilizing Docker Compose.
