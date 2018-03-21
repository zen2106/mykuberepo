Welcome to Dockerizing Spring boot Java App!!!
follow below steps for building Docker images and running Docker containers from images

Steps:

1. Make sure you clone the repo locally.

git clone https://bitbucket.org/ananthkannan/myawesomeangularapprepo

2. once cloned, navigate to repo folder
cd ~/myawesomeangularapprepo/MyAwesomeApp/

3. now run the maven build to make sure you are able to build springboot Jar
mvn clean install

4.once you are able build springboot Jar, next step is build docker images

sudo docker build -t ananthkannan/myspringbootapp . 

5. verify by you have built images successfully
sudo docker images

6. Now run the Docker container from the Docker image you built
sudo docker run -p 8085:8085 ananthkannan/myspringbootapp

7. Now go to browser, and access public DNS name with port 8085
you should see the springboot web app page running
