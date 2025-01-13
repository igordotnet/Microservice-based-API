# Microservice-based-API
 This was a weeklong exercise project in order to obtain a possible internship


## Explanation -
Design a microservice-based API for user management using Docker and PostgreSQL.

## Technical Requirements
* Containerize the application using Docker
* Use PostgreSQL as the database
* Create a Docker Compose configuration
* Implement a robust user management service

# Step-by-step runnin' da code 🏃
* clone the repository (duh)
* On the terminal line run one of the possible docker commands 

1. Build and start the containers
docker-compose up --build

2. To run in detached mode
'docker-compose up -d --build'

After a couple minutes everything should initialize. Once you see a new docker image and its running you should be good to go!

# Checking work

There are two greate ways to check the API 

1. By URL

You should be able to type in 
'http://localhost:3001'
into your browser to see its running and check 'http://localhost:3001' To see all the users 

2. PGAdmin4

If you prefer the Desktop app or Docker Extension you should be able to see the new table created as well as Users (if any are populated)


# Adding/Updating/Checking/Removing Users

I prefer using Postman (a API desktop app) in order to do this. For this exersize I will guide you on creating a user, but to Update-check or Remove users it will be similar steps.

1. Start a New Process
2. In the URL section type 'http://localhost:3001/api/user'
3. Select "POST" from the drop down
4. For the options select the following (Body, Raw, JSON)
5. Input the information of the user you would like to create in JSON standard formating. Here is a example
* '{
    "name": "Testie McGeee",
    "email": "Test@gmail.com"}'
6. You should receive a status of 201, this ensures the data was trasfered successfully
7. Hire me :3

# To stop the containers
docker-compose down