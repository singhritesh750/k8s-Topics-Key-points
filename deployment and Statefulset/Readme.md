# Issue 

1. In Real-world cases we might come accross several hundreds or thousands of microservices running on several hundreds of pods (or to be precise, on containers). So, practically its becomes very tough or sometime nearly impossible to manage those pods and its replicas manually 

2. Eveytime when we have to make any modifications to the pods then first, we had to stop the already running pod and then re-run the pod with new code that was resulting into the downtime for the application which was affecting the customer of the application.

3. Also, another issue arises when we want to recreate pods because of any failure. At that time, writting the command to create a pod with all the options and flags, it becomes very prone to error and also very inefficient way to manage the containers/pods.


So we required a way to use those CRUD operations on pods without having to write everything everytime and also application should be highly Available.
