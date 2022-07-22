run following command to run docker
#docker build -t flask-app-testing .
#docker run --name test-flask -p 5000:5000 flask-app-testing

if you have minikube than use following command
#minikube image load flask-app-testing

#kubectl apply -f k8s/flask_deployment.yaml
#kubectl get deploy

#kubectl get pod

#kubectl logs flask-app-<POD-ID>

For scaling application containers
#kubectl scale deployment flask-app --replicas=6
#kubectl get deploy


for k8s service apply
#kubectl apply -f k8s/flask_service.yaml
#kubectl get svc

for ingress load balancer
#kubectl apply -f k8s/flask_ingress.yaml
#kubectl get ing

For delete kubectl (our app) deployment
#kubectl delete deploy flask-app