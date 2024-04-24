# Jenkins Lab

## yml file
Firts of all, we look up for the docker-compose.yml file and set up the next code:

<img src="images/yml.png"><br>

I opened the port 3000 cause the node feature uses that port and created a volume for persistency. <br>

After that, I used the ```docker-compuse up -d``` command to deploy the container with docker compose and the ```docker exec id_container cat /var/jenkins_home/secrets/initialAdminPassword``` to get the jenkins key
<img src="images/composeup.jpg"><br>

Next, I chosed credentials for my jenkins and the url:
<img src="images/credentials.jpg"><br>
<img src="images/url.jpg"><br>

Then I choose the Nodejs feature for jenkins and hit start jenkins: 
<img src="images/jenkinsconf.jpg"><br>

Now that I had jenkins, I got in the "Administrat Jenkins" field and clicked on tools:
<img src="images/tools.jpg"><br>

In tools, I created a "proyecto estilo libre":
<img src="images/freeproyect.jpg"><br>

Also added my github repository, Node and npm:
<img src="images/git.jpg"><br>
<img src="images/node.jpg"><br>

Finally I got the proyect in my main page and proceeded to execute it:
<img src="images/pipeline.jpg"><br>
<img src="images/working.jpg"><br>