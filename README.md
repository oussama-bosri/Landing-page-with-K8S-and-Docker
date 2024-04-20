Used commands:
docker build -t oussamabs/landingpage .
docker push oussamabs/landingpage
minikube start
kubectl create namespace landingpage
kubectl get namespaces
kubectl -n landingpage apply -f k8s/deployment.yaml
kubectl -n landingpage apply -f k8s/service.yaml
minikube service -n landingpage landingpage --url
