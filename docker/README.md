This will be a experimental docker project form Leonard and Terrapat.

01. Install docker from https://docs.docker.com/install/ good thing about docker it doesn't matter if you have an mac or an windows operating system.

02. After the you installed docker on your machine, you can already run docker commands "very nice". Mac on the terminal, windows on the power-shell

03. Does Docker really works ? Try "docker --version" or even "docker run -it ubuntu bash" in the second command docker downloads a Ubuntu docker image and logs you in as root you can exit by write "exit"

04. After you got the Ubuntu image, you will be inside the docker container. You can notice that the username change to root instead.

05. Use "apt-get -y update" to be able to install apt-get packages. 

06. When you exit the container, all your packages and change will be remoed. If you were to start the docker image again, the container will be from the container which doesn't have our change in it.

07. Do not exit docker before you commit the change in another tabs. It won't saved any change you done in your docker container.

08. WHen you commit, you can see your new image from command "docker images".

09. You can also already availble pull image from docker hub websites with "docker pull <NAME>" 

10. "docker rmi <IMAGE_ID>" to delete the docker image. use "-f"(for force) tag if there are some container using that image.

11. After commiting your docker container and get the new image, you can push the image in your own docker repository (docker cloud)
	- docker login and have to be registered at docker.com
	- docker tag <IMAGE_NAME> <DOCKER_ID_UESR>/<RepositoryName>
	- docker push <DOCKER_ID_USER>/<RepositoryName>
12. You can also pull your repository. Use "docker pull <DOCKER_ID_UESR>/<RepositroyName>" to get your image locally.

13. Then "docker run -ti <IMAGE_ID>" to run the docker container.

14. When not the whole docker image were uploaded and only were the docker file, use docker build -t <REPOSITORY_NAME> .

15. Docker pull will get you the docker image for you, so just use docker run on docker image to run it.


# Reference Links: 

For pulling an image

- https://www.ibm.com/developerworks/community/blogs/8ff122ba-5fbc-4844-8f62-340d437131ee/entry/How_to_build_your_own_Apache_HTTP_server_on_Docker?lang=end 

For running image.

- https://docs.docker.com/engine/reference/run/

For pushing images

- https://docs.docker.com/docker-cloud/builds/push-images/
