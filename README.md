# Mongo-db-configuration using Kubernetes

In this repo, I configured mongo express with mongo database using <b>kubernetes</b>. 

<img width="1215" alt="Screenshot 2022-05-18 at 6 28 00 PM" src="https://user-images.githubusercontent.com/70997750/169044172-351ba817-a558-46bd-aea1-a487300152c1.png">

Components of K8's cluster :

1. Created mongo-db deployment that is connected to following components:
    a. <b> Secrets</b>: The username and password are stored in secrets
    b. <b> Config File </b>: For configuring internal service to the mongo-db pod
    
2. Created internal service <b>(ClusterIP)</b> for routing traffic to the container in the mongo-dp pod

3. Created mongo-express deployment with External service <b>(LoadBalancer)</b> to interact with node

