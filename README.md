# Docker_SSL_Nginx_EC2
TASK 
Deploy dockerised version of a todo API on EC2 with SSL setup. 
So everything from the todo api to nginx to say db should all be running docker containers.

### NOTE
The nginx image used was "jonasal/nginx-certbot:latest"

## You need...
1. An EC2 instance (Ubuntu) with docker and docker-compose installed
2. The instance should have the necessary IAM roles and Security groups to allow SSH, http and https
3. A domain name, use Route 53
4. Clone the repo onto the instance

## List of major things used here
1. dockerfile.1 which is in docker dir
2. api.conf which is in the user_conf.d dir
3. nginx-certbot.env
4. docker-compose.yml
5. .env file