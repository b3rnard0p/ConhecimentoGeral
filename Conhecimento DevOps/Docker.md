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

Windows PowerShell
Copyright (C) Microsoft Corporation. Todos os direitos reservados.

Experimente a nova plataforma cruzada PowerShell https://aka.ms/pscore6

PS C:\Users\Win10> wsl -d ubuntu
To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker
Command 'docker' not found, but can be installed with:
sudo snap install docker
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo apt-get ipdate
[sudo] password for b3rnard0p:
E: Invalid operation ipdate
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo apt-get ipdate
E: Invalid operation ipdate
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo apt-get update
Hit:1 http://archive.ubuntu.com/ubuntu noble InRelease
Get:2 http://archive.ubuntu.com/ubuntu noble-updates InRelease [126 kB]
Get:3 http://security.ubuntu.com/ubuntu noble-security InRelease [126 kB]
Get:4 http://archive.ubuntu.com/ubuntu noble-backports InRelease [126 kB]
Get:5 http://security.ubuntu.com/ubuntu noble-security/main amd64 Packages [670 kB]
Get:6 http://archive.ubuntu.com/ubuntu noble/universe amd64 Packages [15.0 MB]
Get:7 http://security.ubuntu.com/ubuntu noble-security/main Translation-en [130 kB]
Get:8 http://security.ubuntu.com/ubuntu noble-security/main amd64 Components [9004 B]
Get:9 http://security.ubuntu.com/ubuntu noble-security/main amd64 c-n-f Metadata [6912 B]
Get:10 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Packages [819 kB]
Get:11 http://security.ubuntu.com/ubuntu noble-security/universe Translation-en [177 kB]
Get:12 http://security.ubuntu.com/ubuntu noble-security/universe amd64 Components [52.0 kB]
Get:13 http://security.ubuntu.com/ubuntu noble-security/universe amd64 c-n-f Metadata [16.9 kB]
Get:14 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Packages [726 kB]
Get:15 http://security.ubuntu.com/ubuntu noble-security/restricted Translation-en [146 kB]
Get:16 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 Components [208 B]
Get:17 http://security.ubuntu.com/ubuntu noble-security/restricted amd64 c-n-f Metadata [432 B]
Get:18 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Packages [26.2 kB]
Get:19 http://security.ubuntu.com/ubuntu noble-security/multiverse Translation-en [4892 B]
Get:20 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 Components [212 B]
Get:21 http://security.ubuntu.com/ubuntu noble-security/multiverse amd64 c-n-f Metadata [448 B]
Get:22 http://archive.ubuntu.com/ubuntu noble/universe Translation-en [5982 kB]
Get:23 http://archive.ubuntu.com/ubuntu noble/universe amd64 Components [3871 kB]
Get:24 http://archive.ubuntu.com/ubuntu noble/universe amd64 c-n-f Metadata [301 kB]
Get:25 http://archive.ubuntu.com/ubuntu noble/multiverse amd64 Packages [269 kB]
Get:26 http://archive.ubuntu.com/ubuntu noble/multiverse Translation-en [118 kB]
Get:27 http://archive.ubuntu.com/ubuntu noble/multiverse amd64 Components [35.0 kB]
Get:28 http://archive.ubuntu.com/ubuntu noble/multiverse amd64 c-n-f Metadata [8328 B]
Get:29 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 Packages [921 kB]
Get:30 http://archive.ubuntu.com/ubuntu noble-updates/main Translation-en [209 kB]
Get:31 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 Components [151 kB]
Get:32 http://archive.ubuntu.com/ubuntu noble-updates/main amd64 c-n-f Metadata [13.4 kB]
Get:33 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 Packages [1040 kB]
Get:34 http://archive.ubuntu.com/ubuntu noble-updates/universe Translation-en [262 kB]
Get:35 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 Components [364 kB]
Get:36 http://archive.ubuntu.com/ubuntu noble-updates/universe amd64 c-n-f Metadata [25.8 kB]
Get:37 http://archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Packages [759 kB]
Get:38 http://archive.ubuntu.com/ubuntu noble-updates/restricted Translation-en [153 kB]
Get:39 http://archive.ubuntu.com/ubuntu noble-updates/restricted amd64 Components [212 B]
Get:40 http://archive.ubuntu.com/ubuntu noble-updates/restricted amd64 c-n-f Metadata [464 B]
Get:41 http://archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Packages [30.1 kB]
Get:42 http://archive.ubuntu.com/ubuntu noble-updates/multiverse Translation-en [5884 B]
Get:43 http://archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 Components [940 B]
Get:44 http://archive.ubuntu.com/ubuntu noble-updates/multiverse amd64 c-n-f Metadata [656 B]
Get:45 http://archive.ubuntu.com/ubuntu noble-backports/main amd64 Components [208 B]
Get:46 http://archive.ubuntu.com/ubuntu noble-backports/main amd64 c-n-f Metadata [112 B]
Get:47 http://archive.ubuntu.com/ubuntu noble-backports/universe amd64 Packages [14.2 kB]
Get:48 http://archive.ubuntu.com/ubuntu noble-backports/universe Translation-en [12.1 kB]
Get:49 http://archive.ubuntu.com/ubuntu noble-backports/universe amd64 Components [20.0 kB]
Get:50 http://archive.ubuntu.com/ubuntu noble-backports/universe amd64 c-n-f Metadata [1256 B]
Get:51 http://archive.ubuntu.com/ubuntu noble-backports/restricted amd64 Components [216 B]
Get:52 http://archive.ubuntu.com/ubuntu noble-backports/restricted amd64 c-n-f Metadata [116 B]
Get:53 http://archive.ubuntu.com/ubuntu noble-backports/multiverse amd64 Components [212 B]
Get:54 http://archive.ubuntu.com/ubuntu noble-backports/multiverse amd64 c-n-f Metadata [116 B]
Fetched 32.8 MB in 9s (3654 kB/s)
Reading package lists... Done
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo apt-get install ca-certificates curl
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
ca-certificates is already the newest version (20240203).
ca-certificates set to manually installed.
curl is already the newest version (8.5.0-2ubuntu10.6).
curl set to manually installed.
0 upgraded, 0 newly installed, 0 to remove and 56 not upgraded.
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo install -m 0755 -d /etc/apt/keyrings
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo chmod a+r /etc/apt/keyrings/docker.asc
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") stable" | \
> sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo apt-get update
Get:1 https://download.docker.com/linux/ubuntu noble InRelease [48.8 kB]
Get:2 https://download.docker.com/linux/ubuntu noble/stable amd64 Packages [20.3 kB]
Hit:3 http://archive.ubuntu.com/ubuntu noble InRelease
Hit:4 http://archive.ubuntu.com/ubuntu noble-updates InRelease
Hit:5 http://security.ubuntu.com/ubuntu noble-security InRelease
Hit:6 http://archive.ubuntu.com/ubuntu noble-backports InRelease
Fetched 69.2 kB in 1s (50.5 kB/s)
Reading package lists... Done
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  docker-ce-rootless-extras iptables libip4tc2 libip6tc2 libltdl7 libnetfilter-conntrack3 libnfnetlink0 libnftables1
  libnftnl11 libslirp0 nftables pigz slirp4netns
Suggested packages:
  cgroupfs-mount | cgroup-lite firewalld
The following NEW packages will be installed:
  containerd.io docker-buildx-plugin docker-ce docker-ce-cli docker-ce-rootless-extras docker-compose-plugin iptables
  libip4tc2 libip6tc2 libltdl7 libnetfilter-conntrack3 libnfnetlink0 libnftables1 libnftnl11 libslirp0 nftables pigz
  slirp4netns
0 upgraded, 18 newly installed, 0 to remove and 56 not upgraded.
Need to get 121 MB of archives.
After this operation, 442 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 https://download.docker.com/linux/ubuntu noble/stable amd64 containerd.io amd64 1.7.25-1 [29.6 MB]
Get:2 http://archive.ubuntu.com/ubuntu noble/universe amd64 pigz amd64 2.8-1 [65.6 kB]
Get:3 http://archive.ubuntu.com/ubuntu noble/main amd64 libip4tc2 amd64 1.8.10-3ubuntu2 [23.3 kB]
Get:4 http://archive.ubuntu.com/ubuntu noble/main amd64 libip6tc2 amd64 1.8.10-3ubuntu2 [23.7 kB]
Get:5 http://archive.ubuntu.com/ubuntu noble/main amd64 libnfnetlink0 amd64 1.0.2-2build1 [14.8 kB]
Get:6 http://archive.ubuntu.com/ubuntu noble/main amd64 libnetfilter-conntrack3 amd64 1.0.9-6build1 [45.2 kB]
Get:7 http://archive.ubuntu.com/ubuntu noble/main amd64 libnftnl11 amd64 1.2.6-2build1 [66.0 kB]
Get:8 http://archive.ubuntu.com/ubuntu noble/main amd64 iptables amd64 1.8.10-3ubuntu2 [381 kB]
Get:9 http://archive.ubuntu.com/ubuntu noble/main amd64 libnftables1 amd64 1.0.9-1build1 [358 kB]
Get:10 http://archive.ubuntu.com/ubuntu noble/main amd64 nftables amd64 1.0.9-1build1 [69.8 kB]
Get:11 http://archive.ubuntu.com/ubuntu noble/main amd64 libltdl7 amd64 2.4.7-7build1 [40.3 kB]
Get:12 https://download.docker.com/linux/ubuntu noble/stable amd64 docker-buildx-plugin amd64 0.21.1-1~ubuntu.24.04~noble [35.3 MB]
Get:13 http://archive.ubuntu.com/ubuntu noble/main amd64 libslirp0 amd64 4.7.0-1ubuntu3 [63.8 kB]
Get:14 http://archive.ubuntu.com/ubuntu noble/universe amd64 slirp4netns amd64 1.2.1-1build2 [34.9 kB]
Get:15 https://download.docker.com/linux/ubuntu noble/stable amd64 docker-ce-cli amd64 5:28.0.1-1~ubuntu.24.04~noble [15.7 MB]
Get:16 https://download.docker.com/linux/ubuntu noble/stable amd64 docker-ce amd64 5:28.0.1-1~ubuntu.24.04~noble [19.1 MB]
Get:17 https://download.docker.com/linux/ubuntu noble/stable amd64 docker-ce-rootless-extras amd64 5:28.0.1-1~ubuntu.24.04~noble [6086 kB]
Get:18 https://download.docker.com/linux/ubuntu noble/stable amd64 docker-compose-plugin amd64 2.33.1-1~ubuntu.24.04~noble [13.9 MB]
Fetched 121 MB in 10s (11.7 MB/s)
Selecting previously unselected package pigz.
(Reading database ... 40768 files and directories currently installed.)
Preparing to unpack .../00-pigz_2.8-1_amd64.deb ...
Unpacking pigz (2.8-1) ...
Selecting previously unselected package libip4tc2:amd64.
Preparing to unpack .../01-libip4tc2_1.8.10-3ubuntu2_amd64.deb ...
Unpacking libip4tc2:amd64 (1.8.10-3ubuntu2) ...
Selecting previously unselected package libip6tc2:amd64.
Preparing to unpack .../02-libip6tc2_1.8.10-3ubuntu2_amd64.deb ...
Unpacking libip6tc2:amd64 (1.8.10-3ubuntu2) ...
Selecting previously unselected package libnfnetlink0:amd64.
Preparing to unpack .../03-libnfnetlink0_1.0.2-2build1_amd64.deb ...
Unpacking libnfnetlink0:amd64 (1.0.2-2build1) ...
Selecting previously unselected package libnetfilter-conntrack3:amd64.
Preparing to unpack .../04-libnetfilter-conntrack3_1.0.9-6build1_amd64.deb ...
Unpacking libnetfilter-conntrack3:amd64 (1.0.9-6build1) ...
Selecting previously unselected package libnftnl11:amd64.
Preparing to unpack .../05-libnftnl11_1.2.6-2build1_amd64.deb ...
Unpacking libnftnl11:amd64 (1.2.6-2build1) ...
Selecting previously unselected package iptables.
Preparing to unpack .../06-iptables_1.8.10-3ubuntu2_amd64.deb ...
Unpacking iptables (1.8.10-3ubuntu2) ...
Selecting previously unselected package libnftables1:amd64.
Preparing to unpack .../07-libnftables1_1.0.9-1build1_amd64.deb ...
Unpacking libnftables1:amd64 (1.0.9-1build1) ...
Selecting previously unselected package nftables.
Preparing to unpack .../08-nftables_1.0.9-1build1_amd64.deb ...
Unpacking nftables (1.0.9-1build1) ...
Selecting previously unselected package containerd.io.
Preparing to unpack .../09-containerd.io_1.7.25-1_amd64.deb ...
Unpacking containerd.io (1.7.25-1) ...
Selecting previously unselected package docker-buildx-plugin.
Preparing to unpack .../10-docker-buildx-plugin_0.21.1-1~ubuntu.24.04~noble_amd64.deb ...
Unpacking docker-buildx-plugin (0.21.1-1~ubuntu.24.04~noble) ...
Selecting previously unselected package docker-ce-cli.
Preparing to unpack .../11-docker-ce-cli_5%3a28.0.1-1~ubuntu.24.04~noble_amd64.deb ...
Unpacking docker-ce-cli (5:28.0.1-1~ubuntu.24.04~noble) ...
Selecting previously unselected package docker-ce.
Preparing to unpack .../12-docker-ce_5%3a28.0.1-1~ubuntu.24.04~noble_amd64.deb ...
Unpacking docker-ce (5:28.0.1-1~ubuntu.24.04~noble) ...
Selecting previously unselected package docker-ce-rootless-extras.
Preparing to unpack .../13-docker-ce-rootless-extras_5%3a28.0.1-1~ubuntu.24.04~noble_amd64.deb ...
Unpacking docker-ce-rootless-extras (5:28.0.1-1~ubuntu.24.04~noble) ...
Selecting previously unselected package docker-compose-plugin.
Preparing to unpack .../14-docker-compose-plugin_2.33.1-1~ubuntu.24.04~noble_amd64.deb ...
Unpacking docker-compose-plugin (2.33.1-1~ubuntu.24.04~noble) ...
Selecting previously unselected package libltdl7:amd64.
Preparing to unpack .../15-libltdl7_2.4.7-7build1_amd64.deb ...
Unpacking libltdl7:amd64 (2.4.7-7build1) ...
Selecting previously unselected package libslirp0:amd64.
Preparing to unpack .../16-libslirp0_4.7.0-1ubuntu3_amd64.deb ...
Unpacking libslirp0:amd64 (4.7.0-1ubuntu3) ...
Selecting previously unselected package slirp4netns.
Preparing to unpack .../17-slirp4netns_1.2.1-1build2_amd64.deb ...
Unpacking slirp4netns (1.2.1-1build2) ...
Setting up libip4tc2:amd64 (1.8.10-3ubuntu2) ...
Setting up libip6tc2:amd64 (1.8.10-3ubuntu2) ...
Setting up libnftnl11:amd64 (1.2.6-2build1) ...
Setting up docker-buildx-plugin (0.21.1-1~ubuntu.24.04~noble) ...
Setting up containerd.io (1.7.25-1) ...
Created symlink /etc/systemd/system/multi-user.target.wants/containerd.service → /usr/lib/systemd/system/containerd.service.
Setting up docker-compose-plugin (2.33.1-1~ubuntu.24.04~noble) ...
Setting up libltdl7:amd64 (2.4.7-7build1) ...
Setting up docker-ce-cli (5:28.0.1-1~ubuntu.24.04~noble) ...
Setting up libslirp0:amd64 (4.7.0-1ubuntu3) ...
Setting up pigz (2.8-1) ...
Setting up libnfnetlink0:amd64 (1.0.2-2build1) ...
Setting up docker-ce-rootless-extras (5:28.0.1-1~ubuntu.24.04~noble) ...
Setting up libnftables1:amd64 (1.0.9-1build1) ...
Setting up nftables (1.0.9-1build1) ...
Setting up slirp4netns (1.2.1-1build2) ...
Setting up libnetfilter-conntrack3:amd64 (1.0.9-6build1) ...
Setting up iptables (1.8.10-3ubuntu2) ...
update-alternatives: using /usr/sbin/iptables-legacy to provide /usr/sbin/iptables (iptables) in auto mode
update-alternatives: using /usr/sbin/ip6tables-legacy to provide /usr/sbin/ip6tables (ip6tables) in auto mode
update-alternatives: using /usr/sbin/iptables-nft to provide /usr/sbin/iptables (iptables) in auto mode
update-alternatives: using /usr/sbin/ip6tables-nft to provide /usr/sbin/ip6tables (ip6tables) in auto mode
update-alternatives: using /usr/sbin/arptables-nft to provide /usr/sbin/arptables (arptables) in auto mode
update-alternatives: using /usr/sbin/ebtables-nft to provide /usr/sbin/ebtables (ebtables) in auto mode
Setting up docker-ce (5:28.0.1-1~ubuntu.24.04~noble) ...
Created symlink /etc/systemd/system/multi-user.target.wants/docker.service → /usr/lib/systemd/system/docker.service.
Created symlink /etc/systemd/system/sockets.target.wants/docker.socket → /usr/lib/systemd/system/docker.socket.
Processing triggers for man-db (2.12.0-4build2) ...
Processing triggers for libc-bin (2.39-0ubuntu8.4) ...
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker run hello-world
Unable to find image 'hello-world:latest' locally
latest: Pulling from library/hello-world
e6590344b1a5: Pull complete
Digest: sha256:7e1a4e2d11e2ac7a8c3f768d4166c2defeb09d2a750b010412b6ea13de1efb19
Status: Downloaded newer image for hello-world:latest

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker
Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Common Commands:
  run         Create and run a new container from an image
  exec        Execute a command in a running container
  ps          List containers
  build       Build an image from a Dockerfile
  pull        Download an image from a registry
  push        Upload an image to a registry
  images      List images
  login       Authenticate to a registry
  logout      Log out from a registry
  search      Search Docker Hub for images
  version     Show the Docker version information
  info        Display system-wide information

Management Commands:
  builder     Manage builds
  buildx*     Docker Buildx
  checkpoint  Manage checkpoints
  compose*    Docker Compose
  container   Manage containers
  context     Manage contexts
  image       Manage images
  manifest    Manage Docker image manifests and manifest lists
  network     Manage networks
  plugin      Manage plugins
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes

Swarm Commands:
  config      Manage Swarm configs
  node        Manage Swarm nodes
  secret      Manage Swarm secrets
  service     Manage Swarm services
  stack       Manage Swarm stacks
  swarm       Manage Swarm

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  import      Import the contents from a tarball to create a filesystem image
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  wait        Block until one or more containers stop, then print their exit codes

Global Options:
      --config string      Location of client config files (default "/home/b3rnard0p/.docker")
  -c, --context string     Name of the context to use to connect to the daemon (overrides DOCKER_HOST env var and
                           default context set with "docker context use")
  -D, --debug              Enable debug mode
  -H, --host list          Daemon socket to connect to
  -l, --log-level string   Set the logging level ("debug", "info", "warn", "error", "fatal") (default "info")
      --tls                Use TLS; implied by --tlsverify
      --tlscacert string   Trust certs signed only by this CA (default "/home/b3rnard0p/.docker/ca.pem")
      --tlscert string     Path to TLS certificate file (default "/home/b3rnard0p/.docker/cert.pem")
      --tlskey string      Path to TLS key file (default "/home/b3rnard0p/.docker/key.pem")
      --tlsverify          Use TLS and verify the remote
  -v, --version            Print version information and quit

Run 'docker COMMAND --help' for more information on a command.

For more help on how to use Docker, head to https://docs.docker.com/go/guides/
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker container run
docker: 'docker container run' requires at least 1 argument

Usage:  docker container run [OPTIONS] IMAGE [COMMAND] [ARG...]

See 'docker container run --help' for more information
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker container run hello-word
docker: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Head "http://%2Fvar%2Frun%2Fdocker.sock/_ping": dial unix /var/run/docker.sock: connect: permission denied

Run 'docker run --help' for more information
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container run hello-world

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker container ls
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.48/containers/json": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE         COMMAND    CREATED              STATUS                          PORTS     NAMES
3ca5c518fcb9   hello-world   "/hello"   About a minute ago   Exited (0) About a minute ago             loving_euler
827742d50c0a   hello-world   "/hello"   4 minutes ago        Exited (0) 4 minutes ago                  sleepy_neumann
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container run hello-world

Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE         COMMAND    CREATED          STATUS                      PORTS     NAMES
193c17c5f22a   hello-world   "/hello"   12 seconds ago   Exited (0) 12 seconds ago             elegant_keller
3ca5c518fcb9   hello-world   "/hello"   2 minutes ago    Exited (0) 2 minutes ago              loving_euler
827742d50c0a   hello-world   "/hello"   5 minutes ago    Exited (0) 5 minutes ago              sleepy_neumann
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container run postgres
Unable to find image 'postgres:latest' locally
latest: Pulling from library/postgres
6e909acdb790: Pull complete
fec99121872b: Pull complete
133acbc970df: Pull complete
e02d97322fc6: Pull complete
db9643c6baf3: Pull complete
9bcedd9434e7: Pull complete
fc8982ec96d9: Pull complete
1824bd6b75d7: Pull complete
fbad2bf2d5e6: Pull complete
221788d72606: Pull complete
e5f43b682bc0: Pull complete
e7a2d9e24ab0: Pull complete
a96cb29b0d13: Pull complete
140970538145: Pull complete
Digest: sha256:7f29c02ba9eeff4de9a9f414d803faa0e6fe5e8d15ebe217e3e418c82e652b35
Status: Downloaded newer image for postgres:latest
Error: Database is uninitialized and superuser password is not specified.
       You must specify POSTGRES_PASSWORD to a non-empty value for the
       superuser. For example, "-e POSTGRES_PASSWORD=password" on "docker run".

       You may also use "POSTGRES_HOST_AUTH_METHOD=trust" to allow all
       connections without a password. This is *not* recommended.

       See PostgreSQL documentation about "trust":
       https://www.postgresql.org/docs/current/auth-trust.html
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=desafiodocker -e POSTGRES_DB=desafiodocker postgres
docker: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Head "http://%2Fvar%2Frun%2Fdocker.sock/_ping": dial unix /var/run/docker.sock: connect: permission denied

Run 'docker run --help' for more information
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=des
afiodocker -e POSTGRES_DB=desafiodocker postgres
The files belonging to this database system will be owned by user "postgres".
This user must also own the server process.

The database cluster will be initialized with locale "en_US.utf8".
The default database encoding has accordingly been set to "UTF8".
The default text search configuration will be set to "english".

Data page checksums are disabled.

fixing permissions on existing directory /var/lib/postgresql/data ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... posix
selecting default "max_connections" ... 100
selecting default "shared_buffers" ... 128MB
selecting default time zone ... Etc/UTC
creating configuration files ... ok
running bootstrap script ... ok
performing post-bootstrap initialization ... ok
syncing data to disk ... initdb: warning: enabling "trust" authentication for local connections
initdb: hint: You can change this by editing pg_hba.conf or using the option -A, or --auth-local and --auth-host, the next time you run initdb.
ok


Success. You can now start the database server using:

    pg_ctl -D /var/lib/postgresql/data -l logfile start

waiting for server to start....2025-03-19 13:34:29.723 UTC [48] LOG:  starting PostgreSQL 17.4 (Debian 17.4-1.pgdg120+2) on x86_64-pc-linux-gnu, compiled by gcc (Debian 12.2.0-14) 12.2.0, 64-bit
2025-03-19 13:34:29.735 UTC [48] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2025-03-19 13:34:29.745 UTC [51] LOG:  database system was shut down at 2025-03-19 13:34:28 UTC
2025-03-19 13:34:29.754 UTC [48] LOG:  database system is ready to accept connections
 done
server started
CREATE DATABASE


/usr/local/bin/docker-entrypoint.sh: ignoring /docker-entrypoint-initdb.d/*

waiting for server to shut down...2025-03-19 13:34:30.106 UTC [48] LOG:  received fast shutdown request
.2025-03-19 13:34:30.112 UTC [48] LOG:  aborting any active transactions
2025-03-19 13:34:30.113 UTC [48] LOG:  background worker "logical replication launcher" (PID 54) exited with exit code 1
2025-03-19 13:34:30.114 UTC [49] LOG:  shutting down
2025-03-19 13:34:30.129 UTC [49] LOG:  checkpoint starting: shutdown immediate
2025-03-19 13:34:30.568 UTC [49] LOG:  checkpoint complete: wrote 921 buffers (5.6%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.057 s, sync=0.366 s, total=0.455 s; sync files=301, longest=0.130 s, average=0.002 s; distance=4238 kB, estimate=4238 kB; lsn=0/1908980, redo lsn=0/1908980
2025-03-19 13:34:30.574 UTC [48] LOG:  database system is shut down
 done
server stopped

PostgreSQL init process complete; ready for start up.

2025-03-19 13:34:30.650 UTC [1] LOG:  starting PostgreSQL 17.4 (Debian 17.4-1.pgdg120+2) on x86_64-pc-linux-gnu, compiled by gcc (Debian 12.2.0-14) 12.2.0, 64-bit
2025-03-19 13:34:30.650 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
2025-03-19 13:34:30.650 UTC [1] LOG:  listening on IPv6 address "::", port 5432
2025-03-19 13:34:30.658 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2025-03-19 13:34:30.669 UTC [64] LOG:  database system was shut down at 2025-03-19 13:34:30 UTC
2025-03-19 13:34:30.681 UTC [1] LOG:  database system is ready to accept connections
^C2025-03-19 13:35:01.415 UTC [1] LOG:  received fast shutdown request
2025-03-19 13:35:01.422 UTC [1] LOG:  aborting any active transactions
2025-03-19 13:35:01.425 UTC [1] LOG:  background worker "logical replication launcher" (PID 67) exited with exit code 1
2025-03-19 13:35:01.425 UTC [62] LOG:  shutting down
2025-03-19 13:35:01.433 UTC [62] LOG:  checkpoint starting: shutdown immediate
2025-03-19 13:35:01.464 UTC [62] LOG:  checkpoint complete: wrote 4 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.008 s, sync=0.008 s, total=0.040 s; sync files=3, longest=0.005 s, average=0.003 s; distance=0 kB, estimate=0 kB; lsn=0/1908A30, redo lsn=0/1908A30
2025-03-19 13:35:01.468 UTC [1] LOG:  database system is shut down
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE         COMMAND                  CREATED          STATUS                      PORTS     NAMES
ec28a999f3c2   postgres      "docker-entrypoint.s…"   40 seconds ago   Exited (0) 6 seconds ago              friendly_shtern
e0e6b04c1945   postgres      "docker-entrypoint.s…"   6 minutes ago    Exited (1) 6 minutes ago              gifted_chaum
193c17c5f22a   hello-world   "/hello"                 7 minutes ago    Exited (0) 7 minutes ago              elegant_keller
3ca5c518fcb9   hello-world   "/hello"                 10 minutes ago   Exited (0) 10 minutes ago             loving_euler
827742d50c0a   hello-world   "/hello"                 13 minutes ago   Exited (0) 13 minutes ago             sleepy_neumann
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=desafiodocker -e POSTGRES_DB=desafiodocker -d postgres
65363a9d4159fbc253749985d57cd15344444af1571f59cf114675b425e52474
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE         COMMAND                  CREATED              STATUS                      PORTS      NAMES
65363a9d4159   postgres      "docker-entrypoint.s…"   9 seconds ago        Up 9 seconds                5432/tcp   determined_mcnulty
ec28a999f3c2   postgres      "docker-entrypoint.s…"   About a minute ago   Exited (0) 51 seconds ago              friendly_shtern
e0e6b04c1945   postgres      "docker-entrypoint.s…"   6 minutes ago        Exited (1) 6 minutes ago               gifted_chaum
193c17c5f22a   hello-world   "/hello"                 8 minutes ago        Exited (0) 8 minutes ago               elegant_keller
3ca5c518fcb9   hello-world   "/hello"                 11 minutes ago       Exited (0) 11 minutes ago              loving_euler
827742d50c0a   hello-world   "/hello"                 14 minutes ago       Exited (0) 13 minutes ago              sleepy_neumann
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE         COMMAND                  CREATED              STATUS                          PORTS      NAMES
65363a9d4159   postgres      "docker-entrypoint.s…"   19 seconds ago       Up 19 seconds                   5432/tcp   determined_mcnulty
ec28a999f3c2   postgres      "docker-entrypoint.s…"   About a minute ago   Exited (0) About a minute ago              friendly_shtern
e0e6b04c1945   postgres      "docker-entrypoint.s…"   7 minutes ago        Exited (1) 7 minutes ago                   gifted_chaum
193c17c5f22a   hello-world   "/hello"                 8 minutes ago        Exited (0) 8 minutes ago                   elegant_keller
3ca5c518fcb9   hello-world   "/hello"                 11 minutes ago       Exited (0) 11 minutes ago                  loving_euler
827742d50c0a   hello-world   "/hello"                 14 minutes ago       Exited (0) 14 minutes ago                  sleepy_neumann
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container run -e POSTGRES_PASSWORD=Pg@123 -e POSTGRES_USER=desafiodocker -e POSTGRES_DB=desafiodocker -d -p 5432:5432 postgres
4a4104d7625f3cf82f01e58b90c4bab3691dc931a4226e7b6cf333698abd00ee
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls
CONTAINER ID   IMAGE      COMMAND                  CREATED         STATUS         PORTS
        NAMES
4a4104d7625f   postgres   "docker-entrypoint.s…"   8 seconds ago   Up 8 seconds   0.0.0.0:5432->5432/tcp, [::]:5432->5432/tcp   hardcore_dewdney
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls
CONTAINER ID   IMAGE      COMMAND                  CREATED          STATUS          PORTS                                         NAMES
4a4104d7625f   postgres   "docker-entrypoint.s…"   3 minutes ago    Up 3 minutes    0.0.0.0:5432->5432/tcp, [::]:5432->5432/tcp   hardcore_dewdney
65363a9d4159   postgres   "docker-entrypoint.s…"   11 minutes ago   Up 11 minutes   5432/tcp                                      determined_mcnulty
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker container rm 4a4104d7625f
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Delete "http://%2Fvar%2Frun%2Fdocker.sock/v1.48/containers/4a4104d7625f": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker container rm 827742d50c0a
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Delete "http://%2Fvar%2Frun%2Fdocker.sock/v1.48/containers/827742d50c0a": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm 827742d50c0a
827742d50c0a
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm 3ca5c518fcb9
3ca5c518fcb9
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm 193c17c5f22a
193c17c5f22a
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm e0e6b04c1945
e0e6b04c1945
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE      COMMAND                  CREATED          STATUS                      PORTS                                         NAMES
4a4104d7625f   postgres   "docker-entrypoint.s…"   4 minutes ago    Up 4 minutes                0.0.0.0:5432->5432/tcp, [::]:5432->5432/tcp   hardcore_dewdney
65363a9d4159   postgres   "docker-entrypoint.s…"   13 minutes ago   Up 13 minutes               5432/tcp                                      determined_mcnulty
ec28a999f3c2   postgres   "docker-entrypoint.s…"   14 minutes ago   Exited (0) 13 minutes ago                                                 friendly_shtern
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm ec28a999f3c2
ec28a999f3c2
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE      COMMAND                  CREATED          STATUS          PORTS                                         NAMES
4a4104d7625f   postgres   "docker-entrypoint.s…"   4 minutes ago    Up 4 minutes    0.0.0.0:5432->5432/tcp, [::]:5432->5432/tcp   hardcore_dewdney
65363a9d4159   postgres   "docker-entrypoint.s…"   13 minutes ago   Up 13 minutes   5432/tcp                                      determined_mcnulty
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm -f 65363a9d4159
65363a9d4159
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container rm -f 4a4104d7625f
4a4104d7625f
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ git clone https://github.com/fabricioveronez/conversao-distancia.git
Cloning into 'conversao-distancia'...
remote: Enumerating objects: 15, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 15 (delta 4), reused 10 (delta 2), pack-reused 0 (from 0)
Receiving objects: 100% (15/15), 4.56 KiB | 333.00 KiB/s, done.
Resolving deltas: 100% (4/4), done.
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ cd conersao-distancia/
-bash: cd: conersao-distancia/: No such file or directory
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ cd conversao-distancia/
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ code .
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker build -t conversao-distancia .
[sudo] password for b3rnard0p:
[+] Building 74.7s (10/10) FINISHED                                docker:default
 => [internal] load build definition from Dockerfile                         0.1s
 => => transferring dockerfile: 199B                                         0.0s
 => [internal] load metadata for docker.io/library/python:latest             2.4s
 => [internal] load .dockerignore                                            0.1s
 => => transferring context: 2B                                              0.0s
 => [1/5] FROM docker.io/library/python:latest@sha256:8c55c44b9e81d537f840  54.9s
 => => resolve docker.io/library/python:latest@sha256:8c55c44b9e81d537f8404  0.1s
 => => sha256:8c55c44b9e81d537f8404d0000b7331863d134db87c 10.04kB / 10.04kB  0.0s
 => => sha256:7cd785773db44407e20a679ce5439222e505475eed 48.47MB / 48.47MB  22.5s
 => => sha256:255774e0027b72d2327719e78dbad5ad8c9cf446d0 64.40MB / 64.40MB  13.0s
 => => sha256:55a290717432a3298567a9ad264764c63a4dabfef8a94 2.32kB / 2.32kB  0.0s
 => => sha256:e6c8fe2e11080a1bc3b388b235b836d23ce4181cb0f5d 6.26kB / 6.26kB  0.0s
 => => sha256:091eb8249475f42de217265c501e0186f0a3ea7490 24.01MB / 24.01MB  11.0s
 => => sha256:353e14e5cc47664fba714a7da288001d90427c70 211.35MB / 211.35MB  35.7s
 => => sha256:70847531e23db58101b01b1cab1ffdcd984f729cd303 6.16MB / 6.16MB  14.0s
 => => sha256:af0b544b1a82008fe071e025c6a29ca62d3163c270 27.37MB / 27.37MB  18.2s
 => => sha256:379f06e37dbbb740b270a2347c264e3d08bcc5c3037dad45 250B / 250B  18.4s
 => => extracting sha256:7cd785773db44407e20a679ce5439222e505475eed5b99f191  5.7s
 => => extracting sha256:091eb8249475f42de217265c501e0186f0a3ea7490ef7f5145  1.6s
 => => extracting sha256:255774e0027b72d2327719e78dbad5ad8c9cf446d055e45be7  6.4s
 => => extracting sha256:353e14e5cc47664fba714a7da288001d90427c705494847ac  15.1s
 => => extracting sha256:70847531e23db58101b01b1cab1ffdcd984f729cd303049711  0.5s
 => => extracting sha256:af0b544b1a82008fe071e025c6a29ca62d3163c270d921e1a2  1.4s
 => => extracting sha256:379f06e37dbbb740b270a2347c264e3d08bcc5c3037dad4523  0.0s
 => [internal] load build context                                            0.3s
 => => transferring context: 44.12kB                                         0.2s
 => [2/5] WORKDIR /app                                                       1.8s
 => [3/5] COPY requirements.txt .                                            0.2s
 => [4/5] RUN python -m pip install -r requirements.txt                     14.1s
 => [5/5] COPY . .                                                           0.2s
 => exporting to image                                                       0.7s
 => => exporting layers                                                      0.6s
 => => writing image sha256:0368696f7b4456ad8945f3b521e4b35e1edc776bd71173a  0.0s
 => => naming to docker.io/library/conversao-distancia                       0.0s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker build -t conversao-distancia .
[+] Building 1.1s (10/10) FINISHED                                 docker:default
 => [internal] load build definition from Dockerfile                         0.0s
 => => transferring dockerfile: 199B                                         0.0s
 => [internal] load metadata for docker.io/library/python:latest             0.7s
 => [internal] load .dockerignore                                            0.0s
 => => transferring context: 2B                                              0.0s
 => [1/5] FROM docker.io/library/python:latest@sha256:8c55c44b9e81d537f8404  0.0s
 => [internal] load build context                                            0.2s
 => => transferring context: 2.20kB                                          0.2s
 => CACHED [2/5] WORKDIR /app                                                0.0s
 => CACHED [3/5] COPY requirements.txt .                                     0.0s
 => CACHED [4/5] RUN python -m pip install -r requirements.txt               0.0s
 => CACHED [5/5] COPY . .                                                    0.0s
 => exporting to image                                                       0.0s
 => => exporting layers                                                      0.0s
 => => writing image sha256:0368696f7b4456ad8945f3b521e4b35e1edc776bd71173a  0.0s
 => => naming to docker.io/library/conversao-distancia                       0.0s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker cont
ainer run -d -p 5000:5000 conversao-distancia
74109e092b7f8f9fad74d50805aa3aad9ff76fb0d6fbc02badd7acef4e72ab68
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker container ls -a
CONTAINER ID   IMAGE                 COMMAND                  CREATED          STATUS          PORTS                                         NAMES
74109e092b7f   conversao-distancia   "gunicorn --bind 0.0…"   19 seconds ago   Up 18 seconds   0.0.0.0:5000->5000/tcp, [::]:5000->5000/tcp   musing_nash
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ docker image ls
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Head "http://%2Fvar%2Frun%2Fdocker.sock/_ping": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker image ls
REPOSITORY            TAG       IMAGE ID       CREATED          SIZE
conversao-distancia   latest    0368696f7b44   10 minutes ago   1.04GB
postgres              latest    76e3e031d245   2 weeks ago      438MB
hello-world           latest    74cc54e27dc4   8 weeks ago      10.1kB
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ python3 --version
Python 3.12.3
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ docker build -t b3rnar0p/conversao-distancia-desafio:v1
ERROR: docker: 'docker buildx build' requires 1 argument

Usage:  docker buildx build [OPTIONS] PATH | URL | -

Run 'docker buildx build --help' for more information
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker build -t b3rnar0p/conversao-distancia-desafio:v1
ERROR: docker: 'docker buildx build' requires 1 argument

Usage:  docker buildx build [OPTIONS] PATH | URL | -

Run 'docker buildx build --help' for more information
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker build -t b3rnar0p/conversao-distancia-desafio:v1 .
[+] Building 83.7s (10/10) FINISHED                                                                                                                                                               docker:default
 => [internal] load build definition from Dockerfile                                                                                                                                                        0.0s
 => => transferring dockerfile: 206B                                                                                                                                                                        0.0s
 => [internal] load metadata for docker.io/library/python:3.12.3                                                                                                                                            2.3s
 => [internal] load .dockerignore                                                                                                                                                                           0.0s
 => => transferring context: 2B                                                                                                                                                                             0.0s
 => [1/5] FROM docker.io/library/python:3.12.3@sha256:3966b81808d864099f802080d897cef36c01550472ab3955fdd716d1c665acd6                                                                                     52.4s
 => => resolve docker.io/library/python:3.12.3@sha256:3966b81808d864099f802080d897cef36c01550472ab3955fdd716d1c665acd6                                                                                      0.0s
 => => sha256:12e5ab9d51c883bedc4db6c7cbc49f3fa97aef4e98dc205bf1c67e21fd9cb6f4 7.10kB / 7.10kB                                                                                                              0.0s
 => => sha256:c6cf28de8a067787ee0d08f8b01d7f1566a508b56f6e549687b41dfd375f12c7 49.58MB / 49.58MB                                                                                                           17.7s
 => => sha256:891494355808bdd3db5552f0d3723fd0fa826675f774853796fafa221d850d42 24.05MB / 24.05MB                                                                                                           10.3s
 => => sha256:76831bb094456f98613115be37cc8d4f9ab0d128467726ed3160044c80546437 2.01kB / 2.01kB                                                                                                              0.0s
 => => sha256:6582c62583ef22717db8d306b1d6a0c288089ff607d9c0d2d81c4f8973cbfee3 64.14MB / 64.14MB                                                                                                           10.2s
 => => sha256:3966b81808d864099f802080d897cef36c01550472ab3955fdd716d1c665acd6 2.14kB / 2.14kB                                                                                                              0.0s
 => => sha256:bf2c3e352f3d2eed4eda4feeed44a1022a881058df20ac0584db70c138b041e2 211.21MB / 211.21MB                                                                                                         37.4s
 => => sha256:a99509a323905a80628005e4f3bc26ac15ebaf3ffdb08a9646a7f2d110ab38f9 6.39MB / 6.39MB                                                                                                             11.4s
 => => sha256:d46a03def8d9bd846f37fee0edc9fcb7400d68166e99f039cd87b99948af6005 22.69MB / 22.69MB                                                                                                           15.2s
 => => sha256:4429b810e09ef699c3034e49b60f85add3610968983af403fb3181255a5b639f 243B / 243B                                                                                                                 15.5s
 => => sha256:2a4ca5af09fa6cc704c04ba61e304cbf3d0fb2c55f52bf8c8dcba14651216c17 2.77MB / 2.77MB                                                                                                             16.3s
 => => extracting sha256:c6cf28de8a067787ee0d08f8b01d7f1566a508b56f6e549687b41dfd375f12c7                                                                                                                   6.0s
 => => extracting sha256:891494355808bdd3db5552f0d3723fd0fa826675f774853796fafa221d850d42                                                                                                                   4.9s
 => => extracting sha256:6582c62583ef22717db8d306b1d6a0c288089ff607d9c0d2d81c4f8973cbfee3                                                                                                                   6.9s
 => => extracting sha256:bf2c3e352f3d2eed4eda4feeed44a1022a881058df20ac0584db70c138b041e2                                                                                                                  11.4s
 => => extracting sha256:a99509a323905a80628005e4f3bc26ac15ebaf3ffdb08a9646a7f2d110ab38f9                                                                                                                   0.5s
 => => extracting sha256:d46a03def8d9bd846f37fee0edc9fcb7400d68166e99f039cd87b99948af6005                                                                                                                   1.2s
 => => extracting sha256:4429b810e09ef699c3034e49b60f85add3610968983af403fb3181255a5b639f                                                                                                                   0.0s
 => => extracting sha256:2a4ca5af09fa6cc704c04ba61e304cbf3d0fb2c55f52bf8c8dcba14651216c17                                                                                                                   0.4s
 => [internal] load build context                                                                                                                                                                           0.3s
 => => transferring context: 2.38kB                                                                                                                                                                         0.2s
 => [2/5] WORKDIR /app                                                                                                                                                                                     19.1s
 => [3/5] COPY requirements.txt .                                                                                                                                                                           0.1s
 => [4/5] RUN python -m pip install -r requirements.txt                                                                                                                                                     8.7s
 => [5/5] COPY . .                                                                                                                                                                                          0.2s
 => exporting to image                                                                                                                                                                                      0.6s
 => => exporting layers                                                                                                                                                                                     0.4s
 => => writing image sha256:0dc4a0265b0b85fd6665391f75ced0e30cb5b76c852cff6f8c769d18413c1499                                                                                                                0.0s
 => => naming to docker.io/b3rnar0p/conversao-distancia-desafio:v1                                                                                                                                          0.0s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker login

USING WEB-BASED LOGIN

i Info → To sign in with credentials on the command line, use 'docker login -u <username>'


Your one-time device confirmation code is: PKQF-BBGH
Press ENTER to open your browser or submit your device code here: https://login.docker.com/activate

Waiting for authentication in the browser…

WARNING! Your credentials are stored unencrypted in '/root/.docker/config.json'.
Configure a credential helper to remove this warning. See
https://docs.docker.com/go/credential-store/

Login Succeeded
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ docker push b3rnar0p/conversao-distancia-desafio:v1
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Post "http://%2Fvar%2Frun%2Fdocker.sock/v1.48/images/b3rnar0p/conversao-distancia-desafio/push?tag=v1": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker push b3rnar0p/conversao-distancia-desafio:v1
The push refers to repository [docker.io/b3rnar0p/conversao-distancia-desafio]
567b8ae7fa0b: Pushed
6bb0163ae7e7: Pushed
5144de47f930: Pushed
41b01b8398ac: Pushed
490770c36be4: Mounted from library/python
d2533dcba450: Mounted from library/python
ae9947778648: Mounted from library/python
cbe4fb5e267b: Mounted from library/python
734c0f0b65c2: Mounted from library/python
8845ab872c1c: Mounted from library/python
d7d4c2f9d26b: Mounted from library/python
bbe1a212f7e9: Mounted from library/python
v1: digest: sha256:cf652a407672402bc5ab41280262671a6f6aa6c3baeb973f9f776d77b390c1ed size: 2840
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ docker tag b3rnar0p/conversao-distancia-desafio:v1 b3rnar0p/conversao-distancia-desafio:latest
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Post "http://%2Fvar%2Frun%2Fdocker.sock/v1.48/images/b3rnar0p/conversao-distancia-desafio:v1/tag?repo=b3rnar0p%2Fconversao-distancia-desafio&tag=latest": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker tag b3rnar0p/conversao-distancia-desafio:v1 b3rnar0p/conversao-distancia-desafio:latest
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ docker image ls
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Head "http://%2Fvar%2Frun%2Fdocker.sock/_ping": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker image ls
REPOSITORY                             TAG       IMAGE ID       CREATED          SIZE
b3rnar0p/conversao-distancia-desafio   latest    0dc4a0265b0b   3 minutes ago    1.04GB
b3rnar0p/conversao-distancia-desafio   v1        0dc4a0265b0b   3 minutes ago    1.04GB
conversao-distancia                    latest    0368696f7b44   21 minutes ago   1.04GB
postgres                               latest    76e3e031d245   2 weeks ago      438MB
hello-world                            latest    74cc54e27dc4   8 weeks ago      10.1kB
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker push b3rnar0p/conversao-distancia-desafio:latest
The push refers to repository [docker.io/b3rnar0p/conversao-distancia-desafio]
567b8ae7fa0b: Layer already exists
6bb0163ae7e7: Layer already exists
5144de47f930: Layer already exists
41b01b8398ac: Layer already exists
490770c36be4: Layer already exists
d2533dcba450: Layer already exists                                                                                                                                                                               ae9947778648: Layer already exists
cbe4fb5e267b: Layer already exists
734c0f0b65c2: Layer already exists                                                                                                                                                                               8845ab872c1c: Layer already exists
d7d4c2f9d26b: Layer already exists
bbe1a212f7e9: Layer already exists
latest: digest: sha256:cf652a407672402bc5ab41280262671a6f6aa6c3baeb973f9f776d77b390c1ed size: 2840
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker container ls -a
CONTAINER ID   IMAGE                 COMMAND                  CREATED          STATUS          PORTS                                         NAMES
74109e092b7f   conversao-distancia   "gunicorn --bind 0.0…"   19 minutes ago   Up 19 minutes   0.0.0.0:5000->5000/tcp, [::]:5000->5000/tcp   musing_nash
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ docker container rm -f 74109e092b7f
permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Delete "http://%2Fvar%2Frun%2Fdocker.sock/v1.48/containers/74109e092b7f?force=1": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker container rm -f 74109e092b7f
74109e092b7f
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker container ls -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker container run -d -p 5000:5000 b3rnar0p/conversao-distancia-desafio:v1
45f5d2093145339c7839a8dd8b645105d2fbb51dc2d554a21c9d15169af27004
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$ sudo docker container run -d -p 5000:5000 fabricioveronez/conversao-distancia-desafio:v1
Unable to find image 'fabricioveronez/conversao-distancia-desafio:v1' locally
v1: Pulling from fabricioveronez/conversao-distancia-desafio
de4cac68b616: Pull complete
d31b0195ec5f: Pull complete
9b1fd34c30b7: Pull complete
c485c4ba3831: Pull complete
9c94b131279a: Pull complete
30c7a22033ca: Pull complete
69ed005984ad: Pull complete
0aa4295d6be3: Pull complete
8554b361dd86: Pull complete
47dc70fa4714: Pull complete
ea6812a66bba: Pull complete
bb3c78e1c71a: Pull complete
Digest: sha256:9b3b62035b3741c4cd1f18d6c6f5723a6c2b1de679ea95b45d5b5d9933e470c8
Status: Downloaded newer image for fabricioveronez/conversao-distancia-desafio:v1
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/conversao-distancia$



