 

Tuesday, January 31, 2023

6:32 PM

 

 
# Start a Docker Application
navigate to directory, create a jar file
```bash
gradle bootjar
//java -jar ./build/libs/MsdProjectDataServiceFox-0.0.1-SNAPSHOT.jar
//java -jar runs the java program.  do this to make sure the program is //running
```

Build docker images for the services
```bash
docker build --tag dataapi:v1.0 .
OR
docker build --tag reactclient:v1.0 .
```
This builds from the Dockerfile


Start the container, and pass the env variable name if necessary
```bash
docker run -d --name api -p 8080:8080 dataapi:v1.0

examples:
docker run -d --name auth -p 8081:8081 --env API_HOST=172.20.0.2:8080 authapi:v1.0
docker run --name react -it -p 3000:80 reactclient:v1.0
```

Create a network
```bash
docker network create <networkname>
```

Add the container to the network
```bash
docker network connect mccnetwork auth
```

Inspect network to see what is connected
```bash
docker inspect <networkname>
```




Run image/shell

| Docker run \<node\>     |     | Doesn\'t launch interactive version of shell |
|------------------------|---------|----------------------------------------|
| Docker run -it \<node\> |     | Runs interactive version of shell            |

 

 

Show running processes

| Docker ps -a |     | ps = \"processes\" | -a = \"all\" |
|--------------|-----|--------------------|--------------|
