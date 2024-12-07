# react POD
There is a file called react-pod.yaml.
This is the pod related to react container.

# react SERVICE
There is a file called react-service.yaml.
This is the service related to reac pod.
We can't access externally this nginx service without this react-service.yaml.
So we created a nodePort service to access externally.
first port is service port
target port is pod port / container actual port.
node port is the external port when we are trying to access.
There is a option called protocol. If we didnt specify this by default it gets TCP protocol.

# react DELOYEMENT 
deployement file shows the whole diagram of this screnario