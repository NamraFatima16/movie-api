# Agile Software Practice - Assignment 1.

## Movie API

This is a movie API project Which includes:
- **MongoDB** for data storage 
- **Redis** for caching 
- **Mongo Express** for managing the database 

### Project Overview
This application uses Docker compose file to arrange multiple services. Which make it easy to manage the stack locally or in a contained environment.

### Project structure 

The application struction should include:

- **MongoDB**: It stores movies data and make it easy to test.It will contain a seeding that will fill the database when it is set up.
- **Redis**: It reduces the database load and enforces rate only for specific endpoints.
- **Movie API**: It is an API that interacts with MongoDB database and Redis for rated limitations. 
- **Mongo Express**: It uses GUI to view and manage the database. 

### Steps for Launching the Project

1) **Cloning the Repository**

Open bash on your local location 
     git clone https://github.com/NamraFatima16/movie-api.git
     cd movie-api

2) **Installations**

Ensure that you have **Docker** and **Docker Compose** installed on your machine

3) **Launch Stack**
Launch stack by running:
     docker compose up
To launch the stack in a development environment add the --profile dev flag:
     docker compose --profile dev up

4) **Access to Application**
- The API by default listens to 9000 port, so visit http://localhost:9000. to view all the movies navigate to http://localhost:9000/movies.
- The Mongo Express app listens to 8081 port, which can be accessed at http://localhost:8081

### Stopping stack 

To stop the stack run this simple command:
   docker compose down
