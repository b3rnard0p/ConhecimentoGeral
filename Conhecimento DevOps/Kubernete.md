wsl -d ubuntu

docker

curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
  kubectl
  
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl

kubectl

wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash

k3d

sudo k3d cluster create

sudo docker system prune -a --volumes -f

sudo k3d cluster delete k3s-default

sudo k3d cluster create

sudo kubectl get nodes

sudo k3d cluster create --servers 3 --agents 3

sudo docker build -t b3rnar0p/fake-shop-desafio:v1 .

sudo docker push b3rnar0p/fake-shop-desafio:v1

sudo kubectl api-resources

sudo kubectl delete deployment postgre

sudo kubectl apply -f k8s/deployment.yaml

sudo kubectl get pod

sudo kubectl port-forward pod/postgre-68cbd495c7-dr7rt 5432:5432

sudo kubectl port-forward pod/fakeshop-7c896db5d6-4qx5b 5000:500

sudo kubectl logs fakeshop-7c896db5d6-4qx5b

sudo kubectl delete -f k8s/deployment.yaml

sudo kubectl get svc

sudo kubectl port-forward service/fakeshop 5000:5000

sudo k3d cluster delete

sudo k3d cluster create --servers 3 --agents 3 -p "5000:30000@loadbalancer"

sudo kubectl get service

sudo kubectl get deployment

sudo kubectl get replicaset

sudo kubectl get all

sudo kubectl delete pod/fakeshop-5b6b866cf-4ldd4

sudo kubectl get pod -o wide

code ~/.kube/config

kubectl get nodes --context do-nyc1-aula-k8s

sudo k3d cluster stop k3s-default

sudo docker build -t b3rnar0p/fake-shop-desafio:v2 .

sudo docker push b3rnar0p/fake-shop-desafio:v2

kubectl apply -f k8s/deployment.yaml && watch 'kubectl get po'

kubectl get replicaset

kubectl rollout history deployment fakeshop

kubectl rollout undo deployment fakeshop && watch 'kubectl get po'
