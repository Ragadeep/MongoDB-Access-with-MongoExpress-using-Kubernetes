MongoDB-Access-with-MongoExpress-using-Kubernetes

Ustize both Mongo-DB and Mongo Express images

Check The access with in server but outsite minikube cluster
- curl -u [Username]:[Password] http://[Server IP]:[MongoExpress Port]
  
TO Access outside the server. 
- nohup socat TCP-LISTEN:[Port],fork TCP:[minikube IP]:[Port] &

Check the Mongo Express Pod Logs to get the username and password

Access in browser outside the server
- http://[Username]:[Password]@[Server IP]:[MongoExpress Port]
Example of URL : Put decode value of Username and Password
- http://%61%65%6d%69%6e:%70%61%63%73@13.71.61.229:30010
