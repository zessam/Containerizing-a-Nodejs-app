## 0x01-docker-compose

In this section, we will explore using Docker Compose to define and run multi-container applications.

1. Create a `docker-compose.yaml` file in your project directory. This file will define the services, networks, and volumes for your application.

2. Define the necessary services in the `docker-compose.yaml` file. In this case, you need to define the MongoDB and mongo-express services.

3. Start the application using Docker Compose by running the following command in the terminal:

#### To start the application

Step 1: start mongodb and mongo-express

    docker-compose -f docker-compose.yaml up
    
_You can access the mongo-express under localhost:8080 from your browser_
    
Step 2: in mongo-express UI - create a new database "my-db"

Step 3: in mongo-express UI - create a new collection "users" in the database "my-db"       
    
Step 4: start node server 

    cd app
    npm install
    node server.js
    
Step 5: access the nodejs application from browser 

    http://localhost:3000
