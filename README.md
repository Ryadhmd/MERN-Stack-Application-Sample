app-sample

I used the source code provided by the Udemy Course "Docker & Kubernetes: The Practical Guide" (https://www.udemy.com/course/docker-kubernetes-the-practical-guide/) for the purpose of learning and testing Docker and Kubernetes.

The application consists of a MongoDB database, a NodeJS server, and ReactJS. The ReactJS communicates with the NodeJS server through REST API. When users input data, it is stored in the database and the NodeJS server keeps logs about the connection.

To work properly, the application requires the creation of a Docker bridge network where both the MongoDB and the ReactJS will reside. Additionally, the NodeJS port 80 needs to be exposed to allow access to ReactJS, and the ReactJS port 3000 needs to be exposed as well.

In order to make the data persistent, the usage of volumes is necessary. You will find all the commands needed in the docker-commands.txt file and a docker-compose file is provided.

Both the ReactJS and NodeJS are available through Dockerhub:

For NodeJS:

```bash docker pull ryadhamdini/app-sample-nodejs```

For ReactJS:

```bashdocker pull ryadhamdini/app-sample-reactjs```


