# k8s Operation 

1. Ensure minikube has latest images.
2. `kubectl apply -f rabbtmq`. Let rabbitmq boot up. Check logs by calling `kubectl logs queue-0`.
3.  `kubectl apply -f app` to setup api
4.  `kubectl apply -f workers` to setup celery workers.
5.  `kubectl get pods` to get pods and check logs if they are working.
6.  Expose minikube service to view page 
