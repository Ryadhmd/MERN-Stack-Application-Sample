# app-sample
This is an application sample provided by the Udemy Course "Docker & Kubernetes: The Practical Guide" (https://www.udemy.com/course/docker-kubernetes-the-practical-guide/) which I used to learn and test Docker and Kubernetes. 

The application consists of a MongoDB database, a NodeJS server, and ReactJS.
The ReactJS communicates with the NodeJS server through REST API. When users input data, it is stored in the database and the NodeJS server keeps logs about the connection.

To work properly, the application requires the creation of a Docker bridge network where both the MongoDB and the ReactJS will reside. Additionally, the NodeJS port 80 needs to be exposed to allow access to ReactJS, and the ReactJS port 3000 needs to be exposed as well.
In order to make the data persistent, the usage of volumes is necessary.

Both these ReactJS and NodeJS are available throught the Dockerhub : 

For NodeJS :  docker pull ryadhamdini/app-sample-nodejs 

For ReactJS:  docker pull ryadhamdini/app-sample-reactjs 


