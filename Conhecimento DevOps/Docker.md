# 🚀 O que é o Docker?

**Docker** é uma plataforma aberta e de código aberto usada para automatizar o **desenvolvimento, envio e execução de aplicativos** dentro de **contenedores**. Ele permite que os desenvolvedores empacotem uma aplicação e todas as suas dependências em uma única unidade (um contêiner), garantindo que ela seja executada de maneira consistente, independentemente do ambiente em que é executada.

O Docker facilita o processo de **criar, testar e implantar** aplicativos, tornando-o uma ferramenta essencial no desenvolvimento de software moderno, especialmente para **ambientes de microserviços e DevOps**.

## 🏗️ Como Funciona o Docker?

O Docker utiliza contêineres para empacotar o código da aplicação, suas bibliotecas e dependências em uma unidade isolada e reutilizável. Esses contêineres podem ser executados em qualquer máquina que tenha o **Docker instalado**, independentemente do sistema operacional e das configurações locais.

### **Arquitetura do Docker**:

1️⃣ **Imagem Docker**: Uma imagem é uma espécie de "molde" ou template que contém tudo o que é necessário para executar uma aplicação — código, bibliotecas, dependências, variáveis de ambiente e arquivos de configuração. As imagens são imutáveis e podem ser versionadas.

2️⃣ **Contêiner Docker**: O contêiner é uma instância em execução de uma imagem. Ele é **leve e rápido**, com a capacidade de ser iniciado rapidamente e isolado de outros contêineres e do sistema operacional host.

3️⃣ **Docker Engine**: O motor do Docker é o software que executa contêineres e gerencia imagens. Ele pode ser executado tanto em sistemas Linux quanto Windows.

4️⃣ **Docker Hub**: O Docker Hub é um repositório online onde você pode armazenar, compartilhar e obter imagens Docker públicas e privadas.

## 🔄 Como o Docker Facilita o Desenvolvimento?

- **Isolamento e Consistência**: Com o Docker, você pode ter ambientes consistentes e reproduzíveis. Aplicações podem ser testadas e executadas em qualquer lugar com a garantia de que o ambiente será o mesmo.
  
- **Desenvolvimento mais rápido**: O Docker permite que os desenvolvedores criem e testem novas versões de uma aplicação de forma **rápida e eficiente**, além de facilitar o compartilhamento de ambientes de desenvolvimento entre equipes.

- **Escalabilidade**: Com o Docker, é fácil **escalar** aplicações de forma horizontal, criando e gerenciando múltiplos contêineres com a mesma configuração.

## Comandos básicos Docker via terminal WSL

1️⃣ **Inicializar o WSL**:
```
wsl -d ubuntu
```
2️⃣ **Instalar o Docker**:
```
sudo apt-get update

sudo apt-get install ca-certificates curl

sudo install -m 0755 -d /etc/apt/keyrings

sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc

sudo chmod a+r /etc/apt/keyrings/docker.asc

echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
> sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
3️⃣ **Testar se o Docker está funcionando**:
```
sudo docker run hello-world

sudo docker container run hello-world
```
4️⃣ **Listar containers em execução**:
```
sudo docker container ls
```
5️⃣ **Listar todos os containers (inclusive os parados)**:
```
sudo docker container ls -a
```
6️⃣ **Rodar container PostgreSQL com variáveis de ambiente**:
```
sudo docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=des
afiodocker -e POSTGRES_DB=desafiodocker postgres
```
7️⃣ **Rodar PostgreSQL em background (-d)**:
```
sudo docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=desafiodocker -e POSTGRES_DB=desafiodocker -d postgres
```
8️⃣ **Rodar PostgreSQL com mapeamento de porta**:
```
sudo docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=desafiodocker -e POSTGRES_DB=desafiodocker -d -p 5432:5432 postgres
```
9️⃣ **Remover container pelo ID**:
```
sudo docker container rm 827742d50c0a
```
🔟 **Forçar remoção de container pelo ID**:
```
sudo docker container rm -f 4a4104d7625f
```
1️⃣1️⃣ **Clonar repositório do GitHub**:
```
git clone https://github.com/fabricioveronez/conversao-distancia.git

cd conversao-distancia/
code .
```
1️⃣2️⃣ **Construir imagem Docker localmente**:
```
sudo docker build -t conversao-distancia .
```
1️⃣3️⃣ **Rodar container da imagem criada (porta 5000)**:
```
sudo docker container run -d -p 5000:5000 conversao-distancia
```
1️⃣4️⃣  **Listar imagens Docker locais**:
```
sudo docker image ls
```
1️⃣5️⃣ **Construir imagem com nome no Docker Hub**:
```
sudo docker build -t b3rnar0p/conversao-distancia-desafio:v1 .
```
1️⃣6️⃣ **Fazer login no Docker Hub**:
```
sudo docker login
```
1️⃣7️⃣ **Enviar imagem para o Docker Hub**:
```
sudo docker push b3rnar0p/conversao-distancia-desafio:v1
```
1️⃣8️⃣ **Taguear a imagem como latest**:
```
sudo docker tag b3rnar0p/conversao-distancia-desafio:v1 b3rnar0p/conversao-distancia-desafio:latest
```
1️⃣9️⃣ **Enviar imagem latest para Docker Hub**:
```
sudo docker push b3rnar0p/conversao-distancia-desafio:latest
```
2️⃣0️⃣ **Rodar container da imagem enviada (local)**:
```
sudo docker container run -d -p 5000:5000 b3rnar0p/conversao-distancia-desafio:v1
```
2️⃣1️⃣ **Rodar container da imagem de outro repositório**:
```
sudo docker container run -d -p 5000:5000 fabricioveronez/conversao-distancia-desafio:v1
```



