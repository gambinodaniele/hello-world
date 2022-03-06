# pull tomcat

docker images

docker pull tomcat

docker images

# run tomcat on 8081 port

docker run -d --name tomcat-container -p 8081:8080 tomcat

docker ps -a

docker images

# fix container
docker exec -it <container-ID> /bin/bash
cd /user/local/tomcat/webapps.dist
cp . -R * ../webapps/


# create mytomcat-2 image centos + java + timomcat from specific my/Dockerfile

C:\devel\vscode\_java\udemy-devops\hello-world\my>ls
Dockerfile  README.md

C:\devel\vscode\_java\udemy-devops\hello-world\my> docker build -t mytomcat-2 .

docker run -d --name mytomcat-server -p 8083:8080 mytomcat-2