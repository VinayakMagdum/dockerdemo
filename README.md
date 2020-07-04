#Steps to run java application in Docker container.

1.Install Docker
  Fisrt install Docker from official sites.
  And start the docker.

2.Checkout this repository and keep java class and docker file in same folder.

3.Build the docker file to create docker image. You can use below command to
  create docker image.
  docker build .

4.After running this command one docker image gets created.
  To view docker image use following command
  docker images
  The output of this command is as below
  REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
  <none>              <none>              981da1e74ae5        10 sec ago          107MB
  <none>              <none>              f3ceb8444517        5 days ago          107MB
  <none>              <none>              1b3f7cb5a617        12 days ago         108MB
  <none>              <none>              5a9822d4a13b        12 days ago         108MB
  alpine              latest              a24bb4013296        5 weeks ago         5.57MB
  hello-world         latest              bf756fb1ae65        6 months ago        13.3kB

5.Then pick lates image id and use following command
  docker run 981da1e74ae5

6.Then you can get output of you java program. 
