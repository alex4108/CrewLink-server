# Crewlink on Kubernetes

Currently the kubernetes implementation is a single pod scheduled for a single node.  

As the application progresses, it may be possible to run replicas of the pods.

Replace the server name, `ServerNameHere`, with your desired name.

Apply it: `kubectl apply -f http.yml`

The application will be available on port 80 over HTTP at the service's external address.

The pod itself listens on HTTP.  You can configure your load balancer or other reverse proxy to terminate HTTPS traffic destined for the pod.