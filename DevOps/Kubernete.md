# 🚀 O que é o Kubernetes?

**Kubernetes** (ou **K8s**) é uma plataforma **open-source** desenvolvida originalmente pela Google para **automatizar a implantação, o gerenciamento e a escalabilidade de aplicações em contêineres**. Ele orquestra e coordena os contêineres, garantindo que eles sejam executados de maneira eficiente, resiliente e escalável em ambientes de produção.

O Kubernetes é amplamente utilizado em arquiteturas baseadas em **microserviços** e é uma peça-chave em pipelines de **DevOps** e **CI/CD**.

## 🏗️ Como Funciona o Kubernetes?

O Kubernetes gerencia clusters de máquinas (nós) e distribui automaticamente as cargas de trabalho em contêineres nesses nós. Ele cuida de **escalar**, **autocurar** e **distribuir** os serviços conforme as necessidades da aplicação.

### ⚙️ Arquitetura do Kubernetes

1️⃣ **Pod**:  
A menor unidade do Kubernetes. Um Pod pode conter um ou mais contêineres que compartilham o mesmo espaço de rede e armazenamento. É o que o Kubernetes gerencia diretamente para executar os contêineres.

2️⃣ **Node (Nó)**:  
Cada nó é uma máquina (física ou virtual) que faz parte do cluster Kubernetes e que hospeda os Pods. Cada nó possui um **Kubelet** (agente que se comunica com o cluster) e o **runtime** (como Docker ou containerd) para executar os contêineres.

3️⃣ **Cluster**:  
Um conjunto de nós gerenciados pelo **Control Plane** (plano de controle), que é responsável por decidir onde e como os Pods serão distribuídos e escalados.

4️⃣ **Control Plane**:  
O "cérebro" do Kubernetes. Ele contém componentes como o **API Server**, **Scheduler**, **Controller Manager** e o **etcd** (banco de dados distribuído) para controlar o estado desejado do cluster.

5️⃣ **Service**:  
Um recurso do Kubernetes que expõe os Pods para comunicação interna ou externa, garantindo que as aplicações sejam acessíveis dentro ou fora do cluster.

## 🔄 Como o Kubernetes Facilita o Desenvolvimento?

- **Orquestração Automatizada**:  
  O Kubernetes automatiza a distribuição e o agendamento dos contêineres em nós disponíveis, gerenciando a infraestrutura de forma inteligente.

- **Alta Disponibilidade e Autocura**:  
  Se um contêiner ou Pod falhar, o Kubernetes automaticamente cria outro para manter a aplicação em execução.

- **Escalabilidade Dinâmica**:  
  O Kubernetes escala automaticamente os Pods de acordo com a demanda da aplicação, permitindo **escala horizontal** com facilidade.

- **Desacoplamento de Infraestrutura**:  
  As aplicações ficam desacopladas da infraestrutura física ou virtual, permitindo maior portabilidade entre ambientes de desenvolvimento, teste e produção.

---

> 📌 **Observação**: O Kubernetes não substitui o Docker! Na verdade, ele utiliza o Docker (ou outro runtime de contêiner) para executar os contêineres, mas é o Kubernetes que orquestra esses contêineres em larga escala.

## 💻 Comandos Básicos Kubernetes via Terminal (WSL)

Aqui estão alguns comandos essenciais para iniciar, gerenciar e interagir com clusters Kubernetes utilizando o **WSL (Windows Subsystem for Linux)** com **Ubuntu**.

### ⚙️ Preparação e Instalação

1️⃣ **Iniciar o WSL**:
```
wsl -d ubuntu
```
2️⃣ **Instalar o kubectl**:
```
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
kubectl version --client
```
3️⃣ **Instalar o k3d (ferramenta para rodar clusters k3s no Docker)**:
```
wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
k3d version
```

### 🚀 Criação e Gerenciamento de Cluster

4️⃣ **Criar cluster padrão**:
```
sudo k3d cluster create
```
5️⃣ **Excluir cluster padrão**:
```
sudo k3d cluster delete k3s-default
```
6️⃣ **Criar cluster com múltiplos nós**:
```
sudo k3d cluster create --servers 3 --agents 3
```
7️⃣ **Criar cluster com LoadBalancer na porta 5000**:
```
sudo k3d cluster create --servers 3 --agents 3 -p "5000:30000@loadbalancer"
```
8️⃣ **Parar cluster**:
```
sudo k3d cluster stop k3s-default
```

### 🐳 Docker (build & push)

9️⃣ **Limpeza geral do Docker**:
```
sudo docker system prune -a --volumes -f
```
🔟 **Build e push da aplicação**:
```
sudo docker build -t b3rnar0p/fake-shop-desafio:v1 .
sudo docker push b3rnar0p/fake-shop-desafio:v1
```

### 📦 Kubernetes Comandos Essenciais

1️⃣1️⃣ **Listar recursos disponíveis no cluster**:
```
sudo kubectl api-resources
```
1️⃣2️⃣ **Gerenciamento de deploys**:
```
sudo kubectl apply -f k8s/deployment.yaml
sudo kubectl delete -f k8s/deployment.yaml
sudo kubectl delete deployment postgre
```
1️⃣3️⃣ **Verificar pods e serviços**:
```
sudo kubectl get pod
sudo kubectl get svc
sudo kubectl get all
```
1️⃣4️⃣ **Port-forward (expor serviços localmente)**:
```
sudo kubectl port-forward pod/postgre-68cbd495c7-dr7rt 5432:5432
sudo kubectl port-forward pod/fakeshop-7c896db5d6-4qx5b 5000:5000
sudo kubectl port-forward service/fakeshop 5000:5000
```
1️⃣5️⃣ **Ver logs de um pod**:
```
sudo kubectl logs fakeshop-7c896db5d6-4qx5b
```
1️⃣6️⃣ **Outros comandos úteis**:
```
sudo kubectl get deployment
sudo kubectl get replicaset
sudo kubectl get pod -o wide
sudo kubectl delete pod/fakeshop-5b6b866cf-4ldd4
sudo kubectl get nodes
sudo kubectl get nodes --context do-nyc1-aula-k8s
code ~/.kube/config
```
### 🔄 Rollback e Histórico de Deployments

1️⃣7️⃣ **Histórico de rollout**:
```
kubectl rollout history deployment fakeshop
```
1️⃣8️⃣ **Rollback de deployment**:
```
kubectl rollout undo deployment fakeshop && watch 'kubectl get po'
```

### 🚀 Atualização da Aplicação

1️⃣9️⃣ **Build e deploy de nova versão**:
```
sudo docker build -t b3rnar0p/fake-shop-desafio:v2 .
sudo docker push b3rnar0p/fake-shop-desafio:v2
kubectl apply -f k8s/deployment.yaml && watch 'kubectl get po'
```
### Arquivo deployment
```
apiVersion: apps/v1
kind: Deployment
metadata:
  name: postgre
spec:
  selector: 
    matchLabels:
      app: postgre
  template:
    metadata:
      labels:
        app: postgre
    spec:
      containers:
        - name: postgre
          image: postgres:13.16
          ports:
            - containerPort: 5432
          env:
            - name: POSTGRES_PASSWORD
              value: senha
            - name: POSTGRES_USER
              value: ecommerce
            - name: POSTGRES_DB
              value: ecommerce
---

apiVersion: v1
kind: Service
metadata:
  name: postgre
spec:
  type: ClusterIP
  ports:
    - port: 5432
  selector:
    app: postgre
---

apiVersion: apps/v1
kind: Deployment
metadata:
  name: fakeshop
spec:
  replicas: 10
  selector: 
    matchLabels:
      app: fakeshop
  template:
    metadata:
      labels:
        app: fakeshop
    spec:
      containers:
        - name: fakeshop
          image: b3rnar0p/fake-shop-desafio:v2
          ports:
            - containerPort: 5000
          env:
            - name: DB_HOST
              value: postgre
            - name: DB_USER
              value: ecommerce
            - name: DB_PASSWORD
              value: senha
            - name: DB_NAME
              value: ecommerce
            - name: FLASK_APP
              value: index.py
---

apiVersion: v1
kind: Service
metadata:
  name: fakeshop
spec:
  type: LoadBalancer
  ports:
    - port: 80
      targetPort: 5000
      nodePort: 30000
  selector:
    app: fakeshop
```
