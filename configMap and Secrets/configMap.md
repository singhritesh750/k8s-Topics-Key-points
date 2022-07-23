# Issue
If we store the configurations like URLs of service or entrypoint, id, passwords, certs etc. required to connect the deployment, pods, services, Ingress and other components of the k8s to each other on the source code itself then there will be many instances where we don't want to share some of the data with anyone and it will become very unsafe to expose it to public e.g., if we use any SCM (source code manager). 
Also, anaother issue arises when we use those configurations inside the source code is that whenever any of the configuration changes then we have to change all of its traces from all the component's code and that presents very high risk of the hitting errors.

It's then when we required a component where we can put all these configurations at one place and whenever we have to modify it we just have to modify it at one place and it take effect averywhere itself.

# configMap

It is used to store the external configurations.
It stores data in "plain text" format.
It is used to store the data like URLs of service or entrypoint.
