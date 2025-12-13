# To run Web chat App in two ways 
## (Step 1) > Clone the repository.
## Method one (From Docker):
1. If Docker is installed in system.
2. Open terminal in the project directory
> docker build -t webchat-app .
3. Above command will build and create the docker image of project.
> docker compose up
5. Above command will pull and run the required images in containers.

## Method Two (Direct Way):
1. Install and run the redis.
2. Open terminal in the project directory
> pip install -r requirements.txt
3. Above command will install all dependencies required for project.
> daphne webchat.asgi:application
4. Web Application is now running
