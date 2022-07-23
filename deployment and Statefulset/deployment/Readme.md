# deployment

It is used to write all the specifications of the pods like:

1. what containers it should be running inside it.

2. where should it be running.

3. what are their names.

4. metadata etc. 

Simmilar to containers being abstraction over the images, pods being abstraction over the containers, Deployment is abstraction over the pods.

In Real-world cases, we only directly make modifications to the deployment script and all the underlying pods and containers will take effect from it.

Run the commands to apply the changes made to the deployment take effect in the cluster
 
 ```bash
 
 kubectl apply -f [DEPLOYMENT_SCRIPT.YAML]
 
 ```
