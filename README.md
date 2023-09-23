# docker_app_deploy

Process:

 1. Create a GCP linux instance.
 2. Install Docker on it.
 3. Install nginx on it.
 4. Create a directory "myapp" then "cd myapp".
 5. Create a file called "index.html" and add the code (uploaded on Git).
 6. Create a file named Dockerfile and add the code (uploaded on Git).
 7. Build docker image from Dockerfile using "sudo docker build -t myapp ."
 8. Check if the image is properly build using "sudo docker images".
 9. Run docker container from the image using "sudo docker run -d -p 8080:80 myapp".
10. Use "docker ps" to check that your container is running.
11. Add a inbound firewall rule allowing traffic to port 8080.
12. Type the IP_addr:8080. (IP_addr = instance public IP)

Then you can see the frontend of the app that you created. This is hosted on docker container using the custom image created.

Author: Abhilekh Talukdar (M22CS003)
