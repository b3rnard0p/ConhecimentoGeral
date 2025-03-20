Windows PowerShell
Copyright (C) Microsoft Corporation. Todos os direitos reservados.

Experimente a nova plataforma cruzada PowerShell https://aka.ms/pscore6

PS C:\Users\Win10> wsl -d ubuntu
Welcome to Ubuntu 24.04.2 LTS (GNU/Linux 5.15.167.4-microsoft-standard-WSL2 x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/pro

 System information as of Thu Mar 20 09:27:27 -03 2025

  System load:  0.4                 Processes:             58
  Usage of /:   0.6% of 1006.85GB   Users logged in:       0
  Memory usage: 5%                  IPv4 address for eth0: 192.168.153.140
  Swap usage:   0%

 * Strictly confined Kubernetes makes edge and IoT secure. Learn how MicroK8s
   just raised the bar for easy, resilient and secure K8s cluster deployment.

   https://ubuntu.com/engage/secure-kubernetes-at-the-edge

This message is shown once a day. To disable it please create the
/home/b3rnard0p/.hushlogin file.
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
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   138  100   138    0     0    479      0 --:--:-- --:--:-- --:--:--   480
100 54.6M  100 54.6M    0     0  9874k      0  0:00:05  0:00:05 --:--:-- 10.9M
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ kubectl
Command 'kubectl' not found, but can be installed with:
sudo snap install kubectl
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
[sudo] password for b3rnard0p:
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ kubectl
kubectl controls the Kubernetes cluster manager.

 Find more information at: https://kubernetes.io/docs/reference/kubectl/

Basic Commands (Beginner):
  create          Create a resource from a file or from stdin
  expose          Take a replication controller, service, deployment or pod and expose it as a new Kubernetes service
  run             Run a particular image on the cluster
  set             Set specific features on objects

Basic Commands (Intermediate):
  explain         Get documentation for a resource
  get             Display one or many resources
  edit            Edit a resource on the server
  delete          Delete resources by file names, stdin, resources and names, or by resources and label selector

Deploy Commands:
  rollout         Manage the rollout of a resource
  scale           Set a new size for a deployment, replica set, or replication controller
  autoscale       Auto-scale a deployment, replica set, stateful set, or replication controller

Cluster Management Commands:
  certificate     Modify certificate resources
  cluster-info    Display cluster information
  top             Display resource (CPU/memory) usage
  cordon          Mark node as unschedulable
  uncordon        Mark node as schedulable
  drain           Drain node in preparation for maintenance
  taint           Update the taints on one or more nodes

Troubleshooting and Debugging Commands:
  describe        Show details of a specific resource or group of resources
  logs            Print the logs for a container in a pod
  attach          Attach to a running container
  exec            Execute a command in a container
  port-forward    Forward one or more local ports to a pod
  proxy           Run a proxy to the Kubernetes API server
  cp              Copy files and directories to and from containers
  auth            Inspect authorization
  debug           Create debugging sessions for troubleshooting workloads and nodes
  events          List events

Advanced Commands:
  diff            Diff the live version against a would-be applied version
  apply           Apply a configuration to a resource by file name or stdin
  patch           Update fields of a resource
  replace         Replace a resource by file name or stdin
  wait            Experimental: Wait for a specific condition on one or many resources
  kustomize       Build a kustomization target from a directory or URL

Settings Commands:
  label           Update the labels on a resource
  annotate        Update the annotations on a resource
  completion      Output shell completion code for the specified shell (bash, zsh, fish, or powershell)

Subcommands provided by plugins:

Other Commands:
  api-resources   Print the supported API resources on the server
  api-versions    Print the supported API versions on the server, in the form of "group/version"
  config          Modify kubeconfig files
  plugin          Provides utilities for interacting with plugins
  version         Print the client and server version information

Usage:
  kubectl [flags] [options]

Use "kubectl <command> --help" for more information about a given command.
Use "kubectl options" for a list of global command-line options (applies to all commands).
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ wget -q -O - https://raw.githubusercontent.com/k3d-io/k3d/main/install.sh | bash
Preparing to install k3d into /usr/local/bin
k3d installed into /usr/local/bin/k3d
Run 'k3d --help' to see what you can do with it.
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ k3d
Usage:
  k3d [flags]
  k3d [command]

Available Commands:
  cluster      Manage cluster(s)
  completion   Generate completion scripts for [bash, zsh, fish, powershell | psh]
  config       Work with config file(s)
  help         Help about any command
  image        Handle container images.
  kubeconfig   Manage kubeconfig(s)
  node         Manage node(s)
  registry     Manage registry/registries
  version      Show k3d and default k3s version

Flags:
  -h, --help         help for k3d
      --timestamps   Enable Log timestamps
      --trace        Enable super verbose output (trace logging)
      --verbose      Enable verbose output (debug logging)
      --version      Show k3d and default k3s version

Use "k3d [command] --help" for more information about a command.
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ k3d cluster create
ERRO[0000] Failed to get nodes for cluster 'k3s-default': docker failed to get containers with labels 'map[k3d.cluster:k3s-default]': failed to list containers: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/containers/json?all=1&filters=%7B%22label%22%3A%7B%22app%3Dk3d%22%3Atrue%2C%22k3d.cluster%3Dk3s-default%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
INFO[0000] Prep: Network
ERRO[0000] Failed Cluster Preparation: Failed Network Preparation: failed to create cluster network: failed to check for duplicate docker networks: docker failed to list networks: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/networks?filters=%7B%22name%22%3A%7B%22%5E%2F%3Fk3d-k3s-default%24%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
ERRO[0000] Failed to create cluster >>> Rolling Back
INFO[0000] Deleting cluster 'k3s-default'
ERRO[0000] Failed to get nodes for cluster 'k3s-default': docker failed to get containers with labels 'map[k3d.cluster:k3s-default]': failed to list containers: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/containers/json?all=1&filters=%7B%22label%22%3A%7B%22app%3Dk3d%22%3Atrue%2C%22k3d.cluster%3Dk3s-default%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
ERRO[0000] failed to get cluster: No nodes found for given cluster
FATA[0000] Cluster creation FAILED, also FAILED to rollback changes!
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster create
INFO[0000] Prep: Network
INFO[0000] Created network 'k3d-k3s-default'
INFO[0000] Created image volume k3d-k3s-default-images
INFO[0000] Starting new tools node...
INFO[0001] Creating node 'k3d-k3s-default-server-0'
INFO[0001] Pulling image 'ghcr.io/k3d-io/k3d-tools:5.8.3'
INFO[0003] Pulling image 'docker.io/rancher/k3s:v1.31.5-k3s1'
INFO[0004] Starting node 'k3d-k3s-default-tools'
INFO[0016] Creating LoadBalancer 'k3d-k3s-default-serverlb'
INFO[0017] Pulling image 'ghcr.io/k3d-io/k3d-proxy:5.8.3'
INFO[0024] Using the k3d-tools node to gather environment information
INFO[0024] HostIP: using network gateway 172.18.0.1 address
INFO[0024] Starting cluster 'k3s-default'
INFO[0024] Starting servers...
INFO[0024] Starting node 'k3d-k3s-default-server-0'
INFO[0028] All agents already running.
INFO[0028] Starting helpers...
INFO[0028] Starting node 'k3d-k3s-default-serverlb'
INFO[0034] Injecting records for hostAliases (incl. host.k3d.internal) and for 2 network members into CoreDNS configmap...
INFO[0037] Cluster 'k3s-default' created successfully!
INFO[0037] You can now use it like this:
kubectl cluster-info
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ docker_clear
docker_clear: command not found
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker_clear
sudo: docker_clear: command not found
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker system prune -a --volumes -f
Deleted Containers:
f083fb8af39ef9b5ee02f4b2ded5fb4f4f334e48743fe67efad20271d50d6100
45f5d2093145339c7839a8dd8b645105d2fbb51dc2d554a21c9d15169af27004

Deleted Volumes:
5378c81cc031c6edcb2363dd2c58fa2f5a03b5034c8fd07a06d7d8978da8a7e6
933fc195c93f97a627924d9137182baf1319a73ce633470b6f83a9c9ee2bb5e6
0d1268ec35557e43e7ee6290ac9aedc9b2b83adf2b4a20fbbc3adbcdd124204b
619f8d8a829e44518f443fa79fd89e2670757393b9e47af59a73cadc62bb6fef

Deleted Images:
untagged: hello-world:latest
untagged: hello-world@sha256:7e1a4e2d11e2ac7a8c3f768d4166c2defeb09d2a750b010412b6ea13de1efb19
deleted: sha256:74cc54e27dc41bb10dc4b2226072d469509f2f22f1a3ce74f4a59661a1d44602
deleted: sha256:63a41026379f4391a306242eb0b9f26dc3550d863b7fdbb97d899f6eb89efe72
untagged: postgres:latest
untagged: postgres@sha256:7f29c02ba9eeff4de9a9f414d803faa0e6fe5e8d15ebe217e3e418c82e652b35
deleted: sha256:76e3e031d245f3b1018ac3d56a65130a0b7b6c2a55c16b856445a9fb04ddefaf
deleted: sha256:34dba13653a154d83cdf340ed91223f56e172ebfa1e049c7bbe139fbde3314ac
deleted: sha256:5322758e58121b840581203869db9f41541b596864b18a775176d3079765ff3e
deleted: sha256:72eb08b8dafd38c9ebff32ba992900793b63ae1bb8e403c3952b970a25b3a74f
deleted: sha256:bb1249932f5406c6477dff791e1461a1475670bd8fac41623fa59b6c4df20c68
deleted: sha256:ab1a811cfa30750297aff9cd6efac0b875d75f5cbf4c2d4f7fe457762d2e01d9
deleted: sha256:e76f6f3486210f50aff097c536d23458943a44b3222e10ff4833e768cfb3188b
deleted: sha256:58fe591ba71e23c5d369016b9babb2371dc6906565dfb28b1a3ba46a70efa9fc
deleted: sha256:5a70e2eed643e5a976e6e955990656921aa20d147eff2d013eef6bb6e84f348c
deleted: sha256:ea5b9d404e6192310cabbac664c01ef6d421a08128dec2186785f47ec9ebf801
deleted: sha256:3c3f85bd525f63870a32ee31b179bfa891844b969bfe95340b15c932e94fe6de
deleted: sha256:6cabe81fae96d69fe24f67aee0479d832c0ae68d9639e5753a6f2846b2f99d5a
deleted: sha256:66dda6fe1fe2795fac67649338a0278408c89530247ae1c3a76d3e5af02ca347
deleted: sha256:942e092fb5f3fec51cdb3772bb8f74b79c8a4f202f94135838151c13d0129926
deleted: sha256:1287fbecdfcce6ee8cf2436e5b9e9d86a4648db2d91080377d499737f1b307f3
untagged: fabricioveronez/conversao-distancia-desafio:v1
untagged: fabricioveronez/conversao-distancia-desafio@sha256:9b3b62035b3741c4cd1f18d6c6f5723a6c2b1de679ea95b45d5b5d9933e470c8
deleted: sha256:e54a02bdb38453c390089151a558c8645a8beb046960b58d2fb297a4de6050e0
deleted: sha256:120147d6f739e7e2866c71c7a55484c149e2141b27f52a944f301131d0bfebd0
deleted: sha256:594f9c6a9f1f5be278e3fe1426761b6ff0223f297792e7adbd196133f4a028bb
deleted: sha256:c235a397d061f209c42b718c5167e7af5e0cdf99a1e9b699e48aa19a39424e4e
deleted: sha256:0b5d7e52b0de04f1a9b0069d905bbdc0712d8f61465b2aa40f6c0ae286b37940
deleted: sha256:fb65cc20b685c7fa4dd01afb72b716ccf25a8ad515c52dc1e7aa50832edc8058
deleted: sha256:9321db92c8fe327e07a5074d9bd6fef15a647a31494ada81146df78650644f47
deleted: sha256:8db535e7db8acfe97e638a946e0b6e8ca22b2d0f7a25eebc3a8b32449cf7fbe9
deleted: sha256:13f5f07b1f18a4123e9340fc6adb745e6bedbc271d0aa7f12657d401d07110f3
deleted: sha256:77b3ffcd4d50fa908b33901a8a31e1a3983185e0f292a03857076c78adad74c0
deleted: sha256:e381040953511200b742b6b625a07d8f618621a4031c3d276d76d54d66bce1a0
deleted: sha256:f6876fa658c4ab10a996744f0a375893f503f67d4715bf6a3c4a8135b4f2ecfa
deleted: sha256:ff61a9b258e5be019eb30e2ea80b8cefaafb27360a154e5ec0e50f7b9a9cc068
untagged: ghcr.io/k3d-io/k3d-tools:5.8.3
untagged: ghcr.io/k3d-io/k3d-tools@sha256:c5ceb2b9e8ff2cf55917b0bee8bc9c54fe1483a16366b734117e2cfac1417bed
deleted: sha256:8622faa0d552c6339835d00adeaa8b5874694ad530e1650b1748dcd2da89d661
deleted: sha256:19cf4cbfa5344c2acc30c5fbbfe5d7022190115d5c60a1c252d8b2dcb4a546e7
deleted: sha256:149f8fd954d5a84ac225c796f4748bcb4c0a90aa9556fd7824a655cf8080358f
deleted: sha256:c01be9b28516d854e5be0e79ef9a3ea6c2eadf1eab650ee62f59e76c597d8f0e
deleted: sha256:994456c4fd7b2b87346a81961efb4ce945a39592d32e0762b38768bca7c7d085
untagged: conversao-distancia:latest
deleted: sha256:0368696f7b4456ad8945f3b521e4b35e1edc776bd71173a018f42a79bb57fe0f
untagged: b3rnar0p/conversao-distancia-desafio:latest
untagged: b3rnar0p/conversao-distancia-desafio:v1
untagged: b3rnar0p/conversao-distancia-desafio@sha256:cf652a407672402bc5ab41280262671a6f6aa6c3baeb973f9f776d77b390c1ed
deleted: sha256:0dc4a0265b0b85fd6665391f75ced0e30cb5b76c852cff6f8c769d18413c1499

Deleted build cache objects:
pe1tokxieiy3ph9voxjsxrnb1
u5tzefafgwhl0u9lsc9anu2nk
2pdbfmt63t0lfg8yynydficvk
purndni9uvire0ctdmaw3w5dt
li7c8zrkn0ft81ofww91qju0l
3zp6mkhnz8i3zvibk7rqt9ms8
w4a7f2dso19z2ixld0zw90bvj
c7s31op5tko707is2396hemsh
5wni22yg2p6xlgsite69lt5io
bjx6caf7hywkfq0n8bu2w78td
80g9th10pdanz73nrzd4a5gc5
o44esf0rlzhwwbhlqyvba1ral
clcq67z9c4fbge8mfq988v1pd
ygorbc373a25yiyrwwxz4hotp
5ulfi0r3bntj6522sqsrbavjf
0tmex9unof677n7zwvdqiaklj
liodbn4wx6ltxwsigabtz6blx
fg4ox2hiylp6byqhtm7z5sc7k
8donh2409jjd7d04wx8n207uk
2ghzupv0zqz9baadthtp3abg4
huz0lrp2e1rfkuysnxbno81rm
wb4e51hmdzpvur2y9ny1ruscq
npc806oibmaxh1x634ltqi50k
p1a8cq7umpqw9l11y7jlalnzd
y86u90b61jumgzub3rwg9la1n
mb5affox99etch4fiqrw1veor

Total reclaimed space: 1.659GB
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster create
FATA[0000] Failed to create cluster 'k3s-default' because a cluster with that name already exists
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster delete k3s-default
INFO[0000] Deleting cluster 'k3s-default'
INFO[0002] Deleting cluster network 'k3d-k3s-default'
INFO[0002] Deleting 1 attached volumes...
INFO[0002] Removing cluster details from default kubeconfig...
INFO[0002] Removing standalone kubeconfig file (if there is one)...
INFO[0002] Successfully deleted cluster k3s-default!
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster create
INFO[0000] Prep: Network
INFO[0000] Created network 'k3d-k3s-default'
INFO[0000] Created image volume k3d-k3s-default-images
INFO[0000] Starting new tools node...
INFO[0001] Creating node 'k3d-k3s-default-server-0'
INFO[0001] Creating LoadBalancer 'k3d-k3s-default-serverlb'
INFO[0001] Pulling image 'ghcr.io/k3d-io/k3d-tools:5.8.3'
INFO[0004] Starting node 'k3d-k3s-default-tools'
INFO[0004] Using the k3d-tools node to gather environment information
INFO[0005] HostIP: using network gateway 172.18.0.1 address
INFO[0005] Starting cluster 'k3s-default'
INFO[0005] Starting servers...
INFO[0005] Starting node 'k3d-k3s-default-server-0'
INFO[0009] All agents already running.
INFO[0009] Starting helpers...
INFO[0009] Starting node 'k3d-k3s-default-serverlb'
INFO[0015] Injecting records for hostAliases (incl. host.k3d.internal) and for 2 network members into CoreDNS configmap...
INFO[0017] Cluster 'k3s-default' created successfully!
INFO[0017] You can now use it like this:
kubectl cluster-info
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ kubectl get nodes
E0320 09:37:55.242169    5820 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:37:55.243852    5820 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:37:55.245403    5820 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:37:55.247078    5820 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:37:55.249132    5820 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
The connection to the server localhost:8080 was refused - did you specify the right host or port?
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo kubectl get nodes
NAME                       STATUS   ROLES                  AGE   VERSION
k3d-k3s-default-server-0   Ready    control-plane,master   38s   v1.31.5+k3s1
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster list
NAME          SERVERS   AGENTS   LOADBALANCER
k3s-default   1/1       0/0      true
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls
CONTAINER ID   IMAGE                            COMMAND                  CREATED              STATUS              PORTS                             NAMES
86bc2b687d62   ghcr.io/k3d-io/k3d-proxy:5.8.3   "/bin/sh -c nginx-pr…"   About a minute ago   Up About a minute   80/tcp, 0.0.0.0:34439->6443/tcp   k3d-k3s-default-serverlb
e827ad7ec76f   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up About a minute
                            k3d-k3s-default-server-0
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ k3d cluster create --servers 3 --agents 3
ERRO[0000] Failed to get nodes for cluster 'k3s-default': docker failed to get containers with labels 'map[k3d.cluster:k3s-default]': failed to list containers: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/containers/json?all=1&filters=%7B%22label%22%3A%7B%22app%3Dk3d%22%3Atrue%2C%22k3d.cluster%3Dk3s-default%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
INFO[0000] Prep: Network
ERRO[0000] Failed Cluster Preparation: Failed Network Preparation: failed to create cluster network: failed to check for duplicate docker networks: docker failed to list networks: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/networks?filters=%7B%22name%22%3A%7B%22%5E%2F%3Fk3d-k3s-default%24%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
ERRO[0000] Failed to create cluster >>> Rolling Back
INFO[0000] Deleting cluster 'k3s-default'
ERRO[0000] Failed to get nodes for cluster 'k3s-default': docker failed to get containers with labels 'map[k3d.cluster:k3s-default]': failed to list containers: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/containers/json?all=1&filters=%7B%22label%22%3A%7B%22app%3Dk3d%22%3Atrue%2C%22k3d.cluster%3Dk3s-default%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
ERRO[0000] failed to get cluster: No nodes found for given cluster
FATA[0000] Cluster creation FAILED, also FAILED to rollback changes!
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo ]k3d cluster create --servers 3 --agents 3
sudo: ]k3d: command not found
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster create --servers 3 --agents 3
FATA[0000] Failed to create cluster 'k3s-default' because a cluster with that name already exists
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster delete k3s-default
INFO[0000] Deleting cluster 'k3s-default'
INFO[0001] Deleting cluster network 'k3d-k3s-default'
INFO[0002] Deleting 1 attached volumes...
INFO[0002] Removing cluster details from default kubeconfig...
INFO[0002] Removing standalone kubeconfig file (if there is one)...
INFO[0002] Successfully deleted cluster k3s-default!
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo k3d cluster create --servers 3 --agents 3
INFO[0000] Prep: Network
INFO[0000] Created network 'k3d-k3s-default'
INFO[0000] Created image volume k3d-k3s-default-images
INFO[0000] Starting new tools node...
INFO[0000] Creating initializing server node
INFO[0000] Creating node 'k3d-k3s-default-server-0'
INFO[0000] Starting node 'k3d-k3s-default-tools'
INFO[0001] Creating node 'k3d-k3s-default-server-1'
INFO[0002] Creating node 'k3d-k3s-default-server-2'
INFO[0002] Creating node 'k3d-k3s-default-agent-0'
INFO[0002] Creating node 'k3d-k3s-default-agent-1'
INFO[0002] Creating node 'k3d-k3s-default-agent-2'
INFO[0002] Creating LoadBalancer 'k3d-k3s-default-serverlb'
INFO[0002] Using the k3d-tools node to gather environment information
INFO[0003] HostIP: using network gateway 172.18.0.1 address
INFO[0003] Starting cluster 'k3s-default'
INFO[0003] Starting the initializing server...
INFO[0003] Starting node 'k3d-k3s-default-server-0'
INFO[0007] Starting servers...
INFO[0007] Starting node 'k3d-k3s-default-server-1'
INFO[0026] Starting node 'k3d-k3s-default-server-2'
INFO[0043] Starting agents...
INFO[0046] Starting node 'k3d-k3s-default-agent-0'
INFO[0046] Starting node 'k3d-k3s-default-agent-1'
INFO[0046] Starting node 'k3d-k3s-default-agent-2'
INFO[0052] Starting helpers...
INFO[0052] Starting node 'k3d-k3s-default-serverlb'
INFO[0059] Injecting records for hostAliases (incl. host.k3d.internal) and for 7 network members into CoreDNS configmap...
INFO[0061] Cluster 'k3s-default' created successfully!
INFO[0061] You can now use it like this:
kubectl cluster-info
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ kubectl get nodes
E0320 09:41:47.944157   13273 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:41:47.948604   13273 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:41:47.950375   13273 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:41:47.951780   13273 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 09:41:47.953319   13273 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
The connection to the server localhost:8080 was refused - did you specify the right host or port?
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo kubectl get nodes
NAME                       STATUS   ROLES                       AGE   VERSION
k3d-k3s-default-agent-0    Ready    <none>                      23s   v1.31.5+k3s1
k3d-k3s-default-agent-1    Ready    <none>                      23s   v1.31.5+k3s1
k3d-k3s-default-agent-2    Ready    <none>                      22s   v1.31.5+k3s1
k3d-k3s-default-server-0   Ready    control-plane,etcd,master   63s   v1.31.5+k3s1
k3d-k3s-default-server-1   Ready    control-plane,etcd,master   48s   v1.31.5+k3s1
k3d-k3s-default-server-2   Ready    control-plane,etcd,master   30s   v1.31.5+k3s1
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ sudo docker container ls
CONTAINER ID   IMAGE                            COMMAND                  CREATED              STATUS              PORTS                             NAMES
733b2b527757   ghcr.io/k3d-io/k3d-proxy:5.8.3   "/bin/sh -c nginx-pr…"   About a minute ago   Up 36 seconds       80/tcp, 0.0.0.0:35023->6443/tcp   k3d-k3s-default-serverlb
21d53035a95c   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up 42 seconds
                            k3d-k3s-default-agent-2
1cb42fe95462   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up 42 seconds
                            k3d-k3s-default-agent-1
78d32c1f1211   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up 43 seconds
                            k3d-k3s-default-agent-0
23fbc9d5e050   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up About a minute
                            k3d-k3s-default-server-2
36d36d73fad2   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up About a minute
                            k3d-k3s-default-server-1
dd98f7551994   rancher/k3s:v1.31.5-k3s1         "/bin/k3d-entrypoint…"   About a minute ago   Up About a minute
                            k3d-k3s-default-server-0
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ git clone https://github.com/KubeDev/fake-shop.git
Cloning into 'fake-shop'...
remote: Enumerating objects: 187, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (7/7), done.
remote: Total 187 (delta 2), reused 2 (delta 2), pack-reused 178 (from 2)
Receiving objects: 100% (187/187), 687.85 KiB | 2.31 MiB/s, done.
Resolving deltas: 100% (9/9), done.
Updating files: 100% (156/156), done.
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10$ cd fake-shop/
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ code .
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ cd src/
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo docker build -t b3rnar0p/fake-shop-desafio:v1 .
[sudo] password for b3rnard0p:
[+] Building 113.4s (13/13) FINISHED                                                                     docker:default
 => [internal] load build definition from Dockerfile                                                               0.1s
 => => transferring dockerfile: 293B                                                                               0.0s
 => [internal] load metadata for docker.io/library/python:3.11.0                                                   2.5s
 => [auth] library/python:pull token for registry-1.docker.io                                                      0.0s
 => [internal] load .dockerignore                                                                                  0.1s
 => => transferring context: 2B                                                                                    0.0s
 => [1/7] FROM docker.io/library/python:3.11.0@sha256:55101c8373de5311b0ece8746251882ddb0bb394588c93d2477b88852a  92.3s
 => => resolve docker.io/library/python:3.11.0@sha256:55101c8373de5311b0ece8746251882ddb0bb394588c93d2477b88852ad  0.0s
 => => sha256:55101c8373de5311b0ece8746251882ddb0bb394588c93d2477b88852ad00e72 2.14kB / 2.14kB                     0.0s
 => => sha256:2908ae31f385a4c15e9226e1030b63ea2fa91994428abadbfe3e7e373ac03067 2.22kB / 2.22kB                     0.0s
 => => sha256:b9886e761095725d1a1a17007b037cf3a7df594140c54e3580a66608dfd77060 8.52kB / 8.52kB                     0.0s
 => => sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698 55.04MB / 55.04MB                  17.3s
 => => sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037 5.16MB / 5.16MB                     2.6s
 => => sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1 10.88MB / 10.88MB                   3.9s
 => => sha256:094e7d9bb04ebf214ea8dc5a488995449684104ae8ad9603bf061cac0d18eb54 54.59MB / 54.59MB                  24.6s
 => => sha256:2cbfd734f3824a4390fe4be45f6a11a5543bca1023e4814d72460eaebc2eef89 196.87MB / 196.87MB                33.5s
 => => sha256:aa86ac293d0fa66515f0a670445969ba98dd8d6a114a7f6aea934aaad44084d0 6.29MB / 6.29MB                    20.4s
 => => extracting sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698                         10.0s
 => => sha256:32d1faaefc303d530833ba7b47226a58beaea6ac5ba6164bc98d6156b7adb0c3 23.25MB / 23.25MB                  27.8s
 => => sha256:2ccd92605074ba3b14ec8143b014397a9a66a4aeb134a91cdd37f6bed89ded21 233B / 233B                        25.2s
 => => sha256:9a35eb2be5d427970e1e5eda31ebc0c4d825f76db8c21db79a018924f6f4fdc7 3.06MB / 3.06MB                    27.2s
 => => extracting sha256:5c8cfbf51e6e6869f1af2a1e7067b07fd6733036a333c9d29f743b0285e26037                          0.8s
 => => extracting sha256:aa3a609d15798d35c1484072876b7d22a316e98de6a097de33b9dade6a689cd1                          0.9s
 => => extracting sha256:094e7d9bb04ebf214ea8dc5a488995449684104ae8ad9603bf061cac0d18eb54                          6.0s
 => => extracting sha256:2cbfd734f3824a4390fe4be45f6a11a5543bca1023e4814d72460eaebc2eef89                         36.6s
 => => extracting sha256:aa86ac293d0fa66515f0a670445969ba98dd8d6a114a7f6aea934aaad44084d0                          0.9s
 => => extracting sha256:32d1faaefc303d530833ba7b47226a58beaea6ac5ba6164bc98d6156b7adb0c3                          1.3s
 => => extracting sha256:2ccd92605074ba3b14ec8143b014397a9a66a4aeb134a91cdd37f6bed89ded21                          0.0s
 => => extracting sha256:9a35eb2be5d427970e1e5eda31ebc0c4d825f76db8c21db79a018924f6f4fdc7                          0.4s
 => [internal] load build context                                                                                  1.3s
 => => transferring context: 1.69MB                                                                                1.2s
 => [2/7] COPY requirements.txt .                                                                                  1.3s
 => [3/7] RUN python -m pip install -r requirements.txt                                                           13.9s
 => [4/7] WORKDIR /app                                                                                             0.1s
 => [5/7] COPY . /app                                                                                              0.2s
 => [6/7] RUN chmod +x /app/entrypoint.sh                                                                          0.5s
 => [7/7] RUN mkdir -p /tmp/metrics                                                                                0.6s
 => exporting to image                                                                                             1.5s
 => => exporting layers                                                                                            1.3s
 => => writing image sha256:5b8d0f56d43874eeb911a466948b1de0cefc2905ed181ba068a10428af17e4b2                       0.0s
 => => naming to docker.io/b3rnar0p/fake-shop-desafio:v1                                                           0.0s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo docker push b3rnar0p/fake-shop-desafio:v1
The push refers to repository [docker.io/b3rnar0p/fake-shop-desafio]
090a9bb8304b: Pushed
b1b19161070a: Pushed
3bfd4de1b93b: Pushed
42a7de8ccf63: Pushed
a2b78eed1422: Pushed
54c8b000e46c: Pushed
0cd2264d51c3: Mounted from library/python
02bfc2ce10fa: Mounted from library/python
e35157207868: Mounted from library/python
1cad4dc57058: Mounted from library/python
4ff8844d474a: Mounted from library/python
b77487480ddb: Mounted from library/python
cd247c0fb37b: Mounted from library/python
cfdd5c3bd77e: Mounted from library/python
870a241bfebd: Mounted from library/python
v1: digest: sha256:de05ca70c2a502db4f2e7627da6a9298f6c4b69bb8e2f0d90d387a24489dc3d1 size: 3467
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo kubectl api-resource
error: unknown command "api-resource" for "kubectl"

Did you mean this?
        api-resources
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo kubectl api-resources
NAME                                SHORTNAMES   APIVERSION                        NAMESPACED   KIND
bindings                                         v1                                true         Binding
componentstatuses                   cs           v1                                false        ComponentStatus
configmaps                          cm           v1                                true         ConfigMap
endpoints                           ep           v1                                true         Endpoints
events                              ev           v1                                true         Event
limitranges                         limits       v1                                true         LimitRange
namespaces                          ns           v1                                false        Namespace
nodes                               no           v1                                false        Node
persistentvolumeclaims              pvc          v1                                true         PersistentVolumeClaim
persistentvolumes                   pv           v1                                false        PersistentVolume
pods                                po           v1                                true         Pod
podtemplates                                     v1                                true         PodTemplate
replicationcontrollers              rc           v1                                true         ReplicationController
resourcequotas                      quota        v1                                true         ResourceQuota
secrets                                          v1                                true         Secret
serviceaccounts                     sa           v1                                true         ServiceAccount
services                            svc          v1                                true         Service
mutatingwebhookconfigurations                    admissionregistration.k8s.io/v1   false        MutatingWebhookConfiguration
validatingadmissionpolicies                      admissionregistration.k8s.io/v1   false        ValidatingAdmissionPolicy
validatingadmissionpolicybindings                admissionregistration.k8s.io/v1   false        ValidatingAdmissionPolicyBinding
validatingwebhookconfigurations                  admissionregistration.k8s.io/v1   false        ValidatingWebhookConfiguration
customresourcedefinitions           crd,crds     apiextensions.k8s.io/v1           false        CustomResourceDefinition
apiservices                                      apiregistration.k8s.io/v1         false        APIService
controllerrevisions                              apps/v1                           true         ControllerRevision
daemonsets                          ds           apps/v1                           true         DaemonSet
deployments                         deploy       apps/v1                           true         Deployment
replicasets                         rs           apps/v1                           true         ReplicaSet
statefulsets                        sts          apps/v1                           true         StatefulSet
selfsubjectreviews                               authentication.k8s.io/v1          false        SelfSubjectReview
tokenreviews                                     authentication.k8s.io/v1          false        TokenReview
localsubjectaccessreviews                        authorization.k8s.io/v1           true         LocalSubjectAccessReview
selfsubjectaccessreviews                         authorization.k8s.io/v1           false        SelfSubjectAccessReview
selfsubjectrulesreviews                          authorization.k8s.io/v1           false        SelfSubjectRulesReview
subjectaccessreviews                             authorization.k8s.io/v1           false        SubjectAccessReview
horizontalpodautoscalers            hpa          autoscaling/v2                    true         HorizontalPodAutoscaler
cronjobs                            cj           batch/v1                          true         CronJob
jobs                                             batch/v1                          true         Job
certificatesigningrequests          csr          certificates.k8s.io/v1            false        CertificateSigningRequest
leases                                           coordination.k8s.io/v1            true         Lease
endpointslices                                   discovery.k8s.io/v1               true         EndpointSlice
events                              ev           events.k8s.io/v1                  true         Event
flowschemas                                      flowcontrol.apiserver.k8s.io/v1   false        FlowSchema
prioritylevelconfigurations                      flowcontrol.apiserver.k8s.io/v1   false        PriorityLevelConfiguration
helmchartconfigs                                 helm.cattle.io/v1                 true         HelmChartConfig
helmcharts                                       helm.cattle.io/v1                 true         HelmChart
addons                                           k3s.cattle.io/v1                  true         Addon
etcdsnapshotfiles                                k3s.cattle.io/v1                  false        ETCDSnapshotFile
nodes                                            metrics.k8s.io/v1beta1            false        NodeMetrics
pods                                             metrics.k8s.io/v1beta1            true         PodMetrics
ingressclasses                                   networking.k8s.io/v1              false        IngressClass
ingresses                           ing          networking.k8s.io/v1              true         Ingress
networkpolicies                     netpol       networking.k8s.io/v1              true         NetworkPolicy
runtimeclasses                                   node.k8s.io/v1                    false        RuntimeClass
poddisruptionbudgets                pdb          policy/v1                         true         PodDisruptionBudget
clusterrolebindings                              rbac.authorization.k8s.io/v1      false        ClusterRoleBinding
clusterroles                                     rbac.authorization.k8s.io/v1      false        ClusterRole
rolebindings                                     rbac.authorization.k8s.io/v1      true         RoleBinding
roles                                            rbac.authorization.k8s.io/v1      true         Role
priorityclasses                     pc           scheduling.k8s.io/v1              false        PriorityClass
csidrivers                                       storage.k8s.io/v1                 false        CSIDriver
csinodes                                         storage.k8s.io/v1                 false        CSINode
csistoragecapacities                             storage.k8s.io/v1                 true         CSIStorageCapacity
storageclasses                      sc           storage.k8s.io/v1                 false        StorageClass
volumeattachments                                storage.k8s.io/v1                 false        VolumeAttachment
ingressroutes                                    traefik.containo.us/v1alpha1      true         IngressRoute
ingressroutetcps                                 traefik.containo.us/v1alpha1      true         IngressRouteTCP
ingressrouteudps                                 traefik.containo.us/v1alpha1      true         IngressRouteUDP
middlewares                                      traefik.containo.us/v1alpha1      true         Middleware
middlewaretcps                                   traefik.containo.us/v1alpha1      true         MiddlewareTCP
serverstransports                                traefik.containo.us/v1alpha1      true         ServersTransport
tlsoptions                                       traefik.containo.us/v1alpha1      true         TLSOption
tlsstores                                        traefik.containo.us/v1alpha1      true         TLSStore
traefikservices                                  traefik.containo.us/v1alpha1      true         TraefikService
ingressroutes                                    traefik.io/v1alpha1               true         IngressRoute
ingressroutetcps                                 traefik.io/v1alpha1               true         IngressRouteTCP
ingressrouteudps                                 traefik.io/v1alpha1               true         IngressRouteUDP
middlewares                                      traefik.io/v1alpha1               true         Middleware
middlewaretcps                                   traefik.io/v1alpha1               true         MiddlewareTCP
serverstransports                                traefik.io/v1alpha1               true         ServersTransport
serverstransporttcps                             traefik.io/v1alpha1               true         ServersTransportTCP
tlsoptions                                       traefik.io/v1alpha1               true         TLSOption
tlsstores                                        traefik.io/v1alpha1               true         TLSStore
traefikservices                                  traefik.io/v1alpha1               true         TraefikService
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ cd ..
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre created
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          17s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS         RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ErrImagePull   0          35s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          42s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          2m33s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          5m4s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          5m39s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          7m23s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          7m26s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          7m27s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          7m27s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          7m28s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          7m28s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          8m50s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          9m38s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          11m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          15m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS             RESTARTS   AGE
postgre-67f4844d4b-26xdn   0/1     ImagePullBackOff   0          20m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl delete deployment postgre
deployment.apps "postgre" deleted
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre created
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
postgre-68cbd495c7-dr7rt   0/1     ContainerCreating   0          4s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
postgre-68cbd495c7-dr7rt   0/1     ContainerCreating   0          14s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
postgre-68cbd495c7-dr7rt   0/1     ContainerCreating   0          21s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS    RESTARTS   AGE
postgre-68cbd495c7-dr7rt   1/1     Running   0          43s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl port-forward pod/postgre-68cbd495c7-dr7rt 5432:5432
Forwarding from 127.0.0.1:5432 -> 5432
Forwarding from [::1]:5432 -> 5432
Handling connection for 5432
Handling connection for 5432
Handling connection for 5432
Handling connection for 5432
^Cb3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
deployment.apps/fakeshop created
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS              RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   0/1     ContainerCreating   0          8s
postgre-68cbd495c7-dr7rt    1/1     Running             0          8m52s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS              RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   0/1     ContainerCreating   0          17s
postgre-68cbd495c7-dr7rt    1/1     Running             0          9m1s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS              RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   0/1     ContainerCreating   0          28s
postgre-68cbd495c7-dr7rt    1/1     Running             0          9m12s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS              RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   0/1     ContainerCreating   0          35s
postgre-68cbd495c7-dr7rt    1/1     Running             0          9m19s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS              RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   0/1     ContainerCreating   0          60s
postgre-68cbd495c7-dr7rt    1/1     Running             0          9m44s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS    RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   1/1     Running   0          78s
postgre-68cbd495c7-dr7rt    1/1     Running   0          10m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl port-forward pod/fakeshop-7c896db5d6-4qx5b 5000:500
0
Forwarding from 127.0.0.1:5000 -> 5000
Forwarding from [::1]:5000 -> 5000
Handling connection for 5000
Handling connection for 5000
^Cb3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl logs fakeshop-7c896db5d6-4qx5b
Error: Could not locate a Flask application. Use the 'flask --app' option, 'FLASK_APP' environment variable, or a 'wsgi.py' or 'app.py' file in the current directory.

Usage: python -m flask [OPTIONS] COMMAND [ARGS]...
Try 'python -m flask --help' for help.

Error: No such command 'db'.
[2025-03-20 13:50:24 +0000] [8] [INFO] Starting gunicorn 21.0.0
[2025-03-20 13:50:24 +0000] [8] [INFO] Listening at: http://0.0.0.0:5000 (8)
[2025-03-20 13:50:24 +0000] [8] [INFO] Using worker: sync
[2025-03-20 13:50:24 +0000] [9] [INFO] Booting worker with pid: 9
[2025-03-20 13:52:03,825] ERROR in app: Exception on / [GET]
Traceback (most recent call last):
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 145, in __init__
    self._dbapi_connection = engine.raw_connection()
                             ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 3288, in raw_connection
    return self.pool.connect()
           ^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 452, in connect
    return _ConnectionFairy._checkout(self)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 1267, in _checkout
    fairy = _ConnectionRecord.checkout(pool)
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 716, in checkout
    rec = pool._do_get()
          ^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/impl.py", line 169, in _do_get
    with util.safe_reraise():
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py", line 147, in __exit__
    raise exc_value.with_traceback(exc_tb)
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/impl.py", line 167, in _do_get
    return self._create_connection()
           ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 393, in _create_connection
    return _ConnectionRecord(self)
           ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 678, in __init__
    self.__connect()
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 902, in __connect
    with util.safe_reraise():
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py", line 147, in __exit__
    raise exc_value.with_traceback(exc_tb)
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 898, in __connect
    self.dbapi_connection = connection = pool._invoke_creator(self)
                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/create.py", line 637, in connect
    return dialect.connect(*cargs, **cparams)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/default.py", line 615, in connect
    return self.loaded_dbapi.connect(*cargs, **cparams)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/psycopg/connection.py", line 98, in connect
    attempts = conninfo_attempts(params)
               ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/psycopg/_conninfo_attempts.py", line 50, in conninfo_attempts
    raise e.OperationalError(str(last_exc))
psycopg.OperationalError: [Errno -2] Name or service not known

The above exception was the direct cause of the following exception:

Traceback (most recent call last):
  File "/usr/local/lib/python3.11/site-packages/flask/app.py", line 1455, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/flask/app.py", line 869, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/flask/app.py", line 867, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/flask/app.py", line 852, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/app/index.py", line 254, in index
    products = Product.query.all()
               ^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/query.py", line 2692, in all
    return self._iter().all()  # type: ignore
           ^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/query.py", line 2846, in _iter
    result: Union[ScalarResult[_T], Result[_T]] = self.session.execute(
                                                  ^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/session.py", line 2225, in execute
    return self._execute_internal(
           ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/session.py", line 2110, in _execute_internal
    conn = self._connection_for_bind(bind)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/session.py", line 1977, in _connection_for_bind
    return trans._connection_for_bind(engine, execution_options)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "<string>", line 2, in _connection_for_bind
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py", line 136, in _go
    ret_value = fn(self, *arg, **kw)
                ^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/orm/session.py", line 1109, in _connection_for_bind
    conn = bind.connect()
           ^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 3264, in connect
    return self._connection_cls(self)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 147, in __init__
    Connection._handle_dbapi_exception_noconnection(
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 2426, in _handle_dbapi_exception_noconnection
    raise sqlalchemy_exception.with_traceback(exc_info[2]) from e
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 145, in __init__
    self._dbapi_connection = engine.raw_connection()
                             ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/base.py", line 3288, in raw_connection
    return self.pool.connect()
           ^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 452, in connect
    return _ConnectionFairy._checkout(self)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 1267, in _checkout
    fairy = _ConnectionRecord.checkout(pool)
            ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 716, in checkout
    rec = pool._do_get()
          ^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/impl.py", line 169, in _do_get
    with util.safe_reraise():
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py", line 147, in __exit__
    raise exc_value.with_traceback(exc_tb)
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/impl.py", line 167, in _do_get
    return self._create_connection()
           ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 393, in _create_connection
    return _ConnectionRecord(self)
           ^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 678, in __init__
    self.__connect()
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 902, in __connect
    with util.safe_reraise():
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py", line 147, in __exit__
    raise exc_value.with_traceback(exc_tb)
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/pool/base.py", line 898, in __connect
    self.dbapi_connection = connection = pool._invoke_creator(self)
                                         ^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/create.py", line 637, in connect
    return dialect.connect(*cargs, **cparams)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/sqlalchemy/engine/default.py", line 615, in connect
    return self.loaded_dbapi.connect(*cargs, **cparams)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/psycopg/connection.py", line 98, in connect
    attempts = conninfo_attempts(params)
               ^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/usr/local/lib/python3.11/site-packages/psycopg/_conninfo_attempts.py", line 50, in conninfo_attempts
    raise e.OperationalError(str(last_exc))
sqlalchemy.exc.OperationalError: (psycopg.OperationalError) [Errno -2] Name or service not known
(Background on this error at: https://sqlalche.me/e/20/e3q8)
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl delete -f k8s/deployment.yaml
deployment.apps "postgre" deleted
deployment.apps "fakeshop" deleted
Error from server (NotFound): error when deleting "k8s/deployment.yaml": services "postgre" not found
Error from server (NotFound): error when deleting "k8s/deployment.yaml": services "fakeshop" not found
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS        RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   1/1     Terminating   0          12m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS        RESTARTS   AGE
fakeshop-7c896db5d6-4qx5b   1/1     Terminating   0          12m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
No resources found in default namespace.
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre created
service/postgre created
deployment.apps/fakeshop created
service/fakeshop created
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                        READY   STATUS    RESTARTS   AGE
fakeshop-7c896db5d6-npkbh   1/1     Running   0          10s
postgre-68cbd495c7-d4jq7    1/1     Running   0          10s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get svc
NAME         TYPE        CLUSTER-IP    EXTERNAL-IP   PORT(S)          AGE
fakeshop     NodePort    10.43.71.36   <none>        5000:30805/TCP   56s
kubernetes   ClusterIP   10.43.0.1     <none>        443/TCP          82m
postgre      ClusterIP   10.43.2.129   <none>        5432/TCP         56s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl port-forward service/fakeshop 5000:5000
E0320 11:03:58.902990   91034 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 11:03:58.904783   91034 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 11:03:58.906320   91034 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
E0320 11:03:58.907964   91034 memcache.go:265] "Unhandled Error" err="couldn't get current server API group list: Get \"http://localhost:8080/api?timeout=32s\": dial tcp 127.0.0.1:8080: connect: connection refused"
The connection to the server localhost:8080 was refused - did you specify the right host or port?
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl port-forward service/fakeshop 5000:5000
Forwarding from 127.0.0.1:5000 -> 5000
Forwarding from [::1]:5000 -> 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
^Cb3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
service/fakeshop unchanged
The Deployment "fakeshop" is invalid: spec.template.spec.containers[0].env[4].name: Invalid value: "FLASK APP": a valid environment variable name must consist of alphabetic characters, digits, '_', '-', or '.', and must not start with a digit (e.g. 'my.env-name',  or 'MY_ENV.NAME',  or 'MyEnvName1', regex used for validation is '[-._a-zA-Z][-._a-zA-Z0-9]*')
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop configured
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl port-forward service/fakeshop 5000:5000
Forwarding from 127.0.0.1:5000 -> 5000
Forwarding from [::1]:5000 -> 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
Handling connection for 5000
^Cb3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo k3d cluster delete
INFO[0000] Deleting cluster 'k3s-default'
INFO[0010] Deleting cluster network 'k3d-k3s-default'
INFO[0011] Deleting 1 attached volumes...
INFO[0011] Removing cluster details from default kubeconfig...
INFO[0011] Removing standalone kubeconfig file (if there is one)...
INFO[0011] Successfully deleted cluster k3s-default!
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo k3d cluster create --server 3 --agents 3 -p "5000:30000@loa
dbalancer"
Error: unknown flag: --server
Usage:
  k3d cluster create NAME [flags]

Flags:
  -a, --agents int                                                     Specify how many agents you want to create
      --agents-memory string                                           Memory limit imposed on the agents nodes [From docker]
      --api-port [HOST:]HOSTPORT                                       Specify the Kubernetes API server port exposed on the LoadBalancer (Format: [HOST:]HOSTPORT)
                                                                        - Example: `k3d cluster create --servers 3 --api-port 0.0.0.0:6550`
  -c, --config string                                                  Path of a config file to use
  -e, --env KEY[=VALUE][@NODEFILTER[;NODEFILTER...]]                   Add environment variables to nodes (Format: KEY[=VALUE][@NODEFILTER[;NODEFILTER...]]
                                                                        - Example: `k3d cluster create --agents 2 -e "HTTP_PROXY=my.proxy.com@server:0" -e "SOME_KEY=SOME_VAL@server:0"`
      --gpus string                                                    GPU devices to add to the cluster node containers ('all' to pass all GPUs) [From docker]
  -h, --help                                                           help for create
      --host-alias ip:host[,host,...]                                  Add ip:host[,host,...] mappings
      --host-pid-mode                                                  Enable host pid mode of server(s) and agent(s)
  -i, --image string                                                   Specify k3s image that you want to use for the nodes
      --k3s-arg ARG@NODEFILTER[;@NODEFILTER]                           Additional args passed to k3s command (Format: ARG@NODEFILTER[;@NODEFILTER])
                                                                        - Example: `k3d cluster create --k3s-arg "--disable=traefik@server:0"`
      --k3s-node-label KEY[=VALUE][@NODEFILTER[;NODEFILTER...]]        Add label to k3s node (Format: KEY[=VALUE][@NODEFILTER[;NODEFILTER...]]
                                                                        - Example: `k3d cluster create --agents 2 --k3s-node-label "my.label@agent:0,1" --k3s-node-label "other.label=somevalue@server:0"`
      --kubeconfig-switch-context                                      Directly switch the default kubeconfig's current-context to the new cluster's context (requires --kubeconfig-update-default) (default true)
      --kubeconfig-update-default                                      Directly update the default kubeconfig with the new cluster's context (default true)
      --lb-config-override strings                                     Use dotted YAML path syntax to override nginx loadbalancer settings
      --network string                                                 Join an existing network
      --no-image-volume                                                Disable the creation of a volume for importing images
      --no-lb                                                          Disable the creation of a LoadBalancer in front of the server nodes
      --no-rollback                                                    Disable the automatic rollback actions, if anything goes wrong
  -p, --port [HOST:][HOSTPORT:]CONTAINERPORT[/PROTOCOL][@NODEFILTER]   Map ports from the node containers (via the serverlb) to the host (Format: [HOST:][HOSTPORT:]CONTAINERPORT[/PROTOCOL][@NODEFILTER])
                                                                        - Example: `k3d cluster create --agents 2 -p 8080:80@agent:0 -p 8081@agent:1`
      --registry-config string                                         Specify path to an extra registries.yaml file
      --registry-create NAME[:HOST][:HOSTPORT]                         Create a k3d-managed registry and connect it to the cluster (Format: NAME[:HOST][:HOSTPORT]
                                                                        - Example: `k3d cluster create --registry-create mycluster-registry:0.0.0.0:5432`
      --registry-use stringArray                                       Connect to one or more k3d-managed registries running locally
      --runtime-label KEY[=VALUE][@NODEFILTER[;NODEFILTER...]]         Add label to container runtime (Format: KEY[=VALUE][@NODEFILTER[;NODEFILTER...]]
                                                                        - Example: `k3d cluster create --agents 2 --runtime-label "my.label@agent:0,1" --runtime-label "other.label=somevalue@server:0"`
      --runtime-ulimit NAME[=SOFT]:[HARD]                              Add ulimit to container runtime (Format: NAME[=SOFT]:[HARD]
                                                                        - Example: `k3d cluster create --agents 2 --runtime-ulimit "nofile=1024:1024" --runtime-ulimit "noproc=1024:1024"`
  -s, --servers int                                                    Specify how many servers you want to create
      --servers-memory string                                          Memory limit imposed on the server nodes [From docker]
      --subnet 172.28.0.0/16                                           [Experimental: IPAM] Define a subnet for the newly created container network (Example: 172.28.0.0/16)
      --timeout duration                                               Rollback changes if cluster couldn't be created in specified duration.
      --token string                                                   Specify a cluster token. By default, we generate one.
  -v, --volume [SOURCE:]DEST[@NODEFILTER[;NODEFILTER...]]              Mount volumes into the nodes (Format: [SOURCE:]DEST[@NODEFILTER[;NODEFILTER...]]
                                                                        - Example: `k3d cluster create --agents 2 -v /my/path@agent:0,1 -v /tmp/test:/tmp/other@server:0`
      --wait                                                           Wait for the server(s) to be ready before returning. Use '--timeout DURATION' to not wait forever. (default true)

Global Flags:
      --timestamps   Enable Log timestamps
      --trace        Enable super verbose output (trace logging)
      --verbose      Enable verbose output (debug logging)

FATA[0000] unknown flag: --server
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo k3d cluster create --servers 3 --agents 3 -p "5000:30000@lo
adbalancer"
INFO[0000] portmapping '5000:30000' targets the loadbalancer: defaulting to [servers:*:proxy agents:*:proxy]
INFO[0000] Prep: Network
INFO[0000] Created network 'k3d-k3s-default'
INFO[0000] Created image volume k3d-k3s-default-images
INFO[0000] Starting new tools node...
INFO[0000] Creating initializing server node
INFO[0000] Creating node 'k3d-k3s-default-server-0'
INFO[0000] Starting node 'k3d-k3s-default-tools'
INFO[0001] Creating node 'k3d-k3s-default-server-1'
INFO[0002] Creating node 'k3d-k3s-default-server-2'
INFO[0002] Creating node 'k3d-k3s-default-agent-0'
INFO[0002] Creating node 'k3d-k3s-default-agent-1'
INFO[0002] Creating node 'k3d-k3s-default-agent-2'
INFO[0002] Creating LoadBalancer 'k3d-k3s-default-serverlb'
INFO[0002] Using the k3d-tools node to gather environment information
INFO[0003] HostIP: using network gateway 172.18.0.1 address
INFO[0003] Starting cluster 'k3s-default'
INFO[0003] Starting the initializing server...
INFO[0003] Starting node 'k3d-k3s-default-server-0'
INFO[0007] Starting servers...
INFO[0007] Starting node 'k3d-k3s-default-server-1'
INFO[0027] Starting node 'k3d-k3s-default-server-2'
INFO[0057] Starting agents...
INFO[0057] Starting node 'k3d-k3s-default-agent-0'
INFO[0057] Starting node 'k3d-k3s-default-agent-2'
INFO[0057] Starting node 'k3d-k3s-default-agent-1'
INFO[0063] Starting helpers...
INFO[0063] Starting node 'k3d-k3s-default-serverlb'
INFO[0070] Injecting records for hostAliases (incl. host.k3d.internal) and for 7 network members into CoreDNS configmap...
INFO[0072] Cluster 'k3s-default' created successfully!
INFO[0072] You can now use it like this:
kubectl cluster-info
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre created
service/postgre created
deployment.apps/fakeshop created
service/fakeshop created
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-4ldd4   0/1     ContainerCreating   0          16s
postgre-68cbd495c7-vt2k9   0/1     ContainerCreating   0          16s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get service
NAME         TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
fakeshop     NodePort    10.43.66.179   <none>        5000:30904/TCP   27s
kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          112s
postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         27s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop unchanged
service/fakeshop configured
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS    RESTARTS   AGE
fakeshop-5b6b866cf-4ldd4   1/1     Running   0          81s
postgre-68cbd495c7-vt2k9   1/1     Running   0          81s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get service
NAME         TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   84s
kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          2m49s
postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         84s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get deployment
NAME       READY   UP-TO-DATE   AVAILABLE   AGE
fakeshop   1/1     1            1           2m54s
postgre    1/1     1            1           2m54s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get replicaset
NAME                 DESIRED   CURRENT   READY   AGE
fakeshop-5b6b866cf   1         1         1       3m4s
postgre-68cbd495c7   1         1         1       3m4s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
NAME                           READY   STATUS    RESTARTS   AGE
pod/fakeshop-5b6b866cf-4ldd4   1/1     Running   0          4m22s
pod/postgre-68cbd495c7-vt2k9   1/1     Running   0          4m22s

NAME                 TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   4m22s
service/kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          5m47s
service/postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         4m22s

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   1/1     1            1           4m22s
deployment.apps/postgre    1/1     1            1           4m22s

NAME                                 DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5b6b866cf   1         1         1       4m22s
replicaset.apps/postgre-68cbd495c7   1         1         1       4m22s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl dele pod/fakeshop-5b6b866cf-4ldd4
error: unknown command "dele" for "kubectl"

Did you mean this?
        delete
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl delete pod/fakeshop-5b6b866cf-4ldd4
pod "fakeshop-5b6b866cf-4ldd4" deleted
^Cb3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-4ldd4   1/1     Terminating         0          5m38s
fakeshop-5b6b866cf-bsmfq   0/1     ContainerCreating   0          26s
postgre-68cbd495c7-vt2k9   1/1     Running             0          5m38s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-4ldd4   1/1     Terminating         0          5m52s
fakeshop-5b6b866cf-bsmfq   0/1     ContainerCreating   0          40s
postgre-68cbd495c7-vt2k9   1/1     Running             0          5m52s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
NAME                           READY   STATUS              RESTARTS   AGE
pod/fakeshop-5b6b866cf-bsmfq   0/1     ContainerCreating   0          53s
pod/postgre-68cbd495c7-vt2k9   1/1     Running             0          6m5s

NAME                 TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   6m6s
service/kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          7m31s
service/postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         6m6s

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   0/1     1            0           6m6s
deployment.apps/postgre    1/1     1            1           6m6s

NAME                                 DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5b6b866cf   1         1         0       6m6s
replicaset.apps/postgre-68cbd495c7   1         1         1       6m6s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS    RESTARTS   AGE
fakeshop-5b6b866cf-bsmfq   1/1     Running   0          66s
postgre-68cbd495c7-vt2k9   1/1     Running   0          6m18s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
NAME                           READY   STATUS    RESTARTS   AGE
pod/fakeshop-5b6b866cf-bsmfq   1/1     Running   0          69s
pod/postgre-68cbd495c7-vt2k9   1/1     Running   0          6m21s

NAME                 TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   6m21s
service/kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          7m46s
service/postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         6m21s

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   1/1     1            1           6m21s
deployment.apps/postgre    1/1     1            1           6m21s

NAME                                 DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5b6b866cf   1         1         1       6m21s
replicaset.apps/postgre-68cbd495c7   1         1         1       6m21s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop configured
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-bsmfq   1/1     Running             0          107s
fakeshop-5b6b866cf-chxx5   0/1     ContainerCreating   0          7s
fakeshop-5b6b866cf-ck7k8   0/1     ContainerCreating   0          7s
fakeshop-5b6b866cf-ggztd   1/1     Running             0          7s
fakeshop-5b6b866cf-h6n55   0/1     ContainerCreating   0          7s
fakeshop-5b6b866cf-hplw9   0/1     ContainerCreating   0          7s
fakeshop-5b6b866cf-k5p5v   1/1     Running             0          7s
fakeshop-5b6b866cf-ms68f   1/1     Running             0          7s
fakeshop-5b6b866cf-tgqpm   0/1     ContainerCreating   0          8s
fakeshop-5b6b866cf-zlg65   0/1     ContainerCreating   0          7s
postgre-68cbd495c7-vt2k9   1/1     Running             0          6m59s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-bsmfq   1/1     Running             0          2m6s
fakeshop-5b6b866cf-chxx5   0/1     ContainerCreating   0          26s
fakeshop-5b6b866cf-ck7k8   0/1     ContainerCreating   0          26s
fakeshop-5b6b866cf-ggztd   1/1     Running             0          26s
fakeshop-5b6b866cf-h6n55   0/1     ContainerCreating   0          26s
fakeshop-5b6b866cf-hplw9   0/1     ContainerCreating   0          26s
fakeshop-5b6b866cf-k5p5v   1/1     Running             0          26s
fakeshop-5b6b866cf-ms68f   1/1     Running             0          26s
fakeshop-5b6b866cf-tgqpm   0/1     ContainerCreating   0          27s
fakeshop-5b6b866cf-zlg65   0/1     ContainerCreating   0          26s
postgre-68cbd495c7-vt2k9   1/1     Running             0          7m18s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl delete pod/fakeshop-5b6b866cf-ggztd
pod "fakeshop-5b6b866cf-ggztd" deleted
^Cb3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-bsmfq   1/1     Running             0          2m36s
fakeshop-5b6b866cf-cd7dt   1/1     Running             0          8s
fakeshop-5b6b866cf-chxx5   0/1     ContainerCreating   0          56s
fakeshop-5b6b866cf-ck7k8   0/1     ContainerCreating   0          56s
fakeshop-5b6b866cf-ggztd   1/1     Terminating         0          56s
fakeshop-5b6b866cf-h6n55   0/1     ContainerCreating   0          56s
fakeshop-5b6b866cf-hplw9   0/1     ContainerCreating   0          56s
fakeshop-5b6b866cf-k5p5v   1/1     Running             0          56s
fakeshop-5b6b866cf-ms68f   1/1     Running             0          56s
fakeshop-5b6b866cf-tgqpm   0/1     ContainerCreating   0          57s
fakeshop-5b6b866cf-zlg65   0/1     ContainerCreating   0          56s
postgre-68cbd495c7-vt2k9   1/1     Running             0          7m48s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-bsmfq   1/1     Running             0          3m8s
fakeshop-5b6b866cf-cd7dt   1/1     Running             0          40s
fakeshop-5b6b866cf-chxx5   0/1     ContainerCreating   0          88s
fakeshop-5b6b866cf-ck7k8   0/1     ContainerCreating   0          88s
fakeshop-5b6b866cf-ggztd   1/1     Terminating         0          88s
fakeshop-5b6b866cf-h6n55   0/1     ContainerCreating   0          88s
fakeshop-5b6b866cf-hplw9   0/1     ContainerCreating   0          88s
fakeshop-5b6b866cf-k5p5v   1/1     Running             0          88s
fakeshop-5b6b866cf-ms68f   1/1     Running             0          88s
fakeshop-5b6b866cf-tgqpm   0/1     ContainerCreating   0          89s
fakeshop-5b6b866cf-zlg65   0/1     ContainerCreating   0          88s
postgre-68cbd495c7-vt2k9   1/1     Running             0          8m20s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod
NAME                       READY   STATUS              RESTARTS   AGE
fakeshop-5b6b866cf-bsmfq   1/1     Running             0          4m4s
fakeshop-5b6b866cf-cd7dt   1/1     Running             0          96s
fakeshop-5b6b866cf-chxx5   0/1     ContainerCreating   0          2m24s
fakeshop-5b6b866cf-ck7k8   0/1     ContainerCreating   0          2m24s
fakeshop-5b6b866cf-h6n55   0/1     ContainerCreating   0          2m24s
fakeshop-5b6b866cf-hplw9   0/1     ContainerCreating   0          2m24s
fakeshop-5b6b866cf-k5p5v   1/1     Running             0          2m24s
fakeshop-5b6b866cf-ms68f   1/1     Running             0          2m24s
fakeshop-5b6b866cf-tgqpm   0/1     ContainerCreating   0          2m25s
fakeshop-5b6b866cf-zlg65   0/1     ContainerCreating   0          2m24s
postgre-68cbd495c7-vt2k9   1/1     Running             0          9m16s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get pod -o wide
NAME                       READY   STATUS              RESTARTS   AGE     IP          NODE                       NOMINATED NODE   READINESS GATES
fakeshop-5b6b866cf-bsmfq   1/1     Running             0          4m32s   10.42.4.3   k3d-k3s-default-agent-0    <none>           <none>
fakeshop-5b6b866cf-cd7dt   1/1     Running             0          2m4s    10.42.6.6   k3d-k3s-default-agent-1    <none>           <none>
fakeshop-5b6b866cf-chxx5   0/1     ContainerCreating   0          2m52s   <none>      k3d-k3s-default-server-0   <none>           <none>
fakeshop-5b6b866cf-ck7k8   1/1     Running             0          2m52s   10.42.5.4   k3d-k3s-default-agent-2    <none>           <none>
fakeshop-5b6b866cf-h6n55   1/1     Running             0          2m52s   10.42.3.5   k3d-k3s-default-server-2   <none>           <none>
fakeshop-5b6b866cf-hplw9   1/1     Running             0          2m52s   10.42.3.4   k3d-k3s-default-server-2   <none>           <none>
fakeshop-5b6b866cf-k5p5v   1/1     Running             0          2m52s   10.42.6.4   k3d-k3s-default-agent-1    <none>           <none>
fakeshop-5b6b866cf-ms68f   1/1     Running             0          2m52s   10.42.4.4   k3d-k3s-default-agent-0    <none>           <none>
fakeshop-5b6b866cf-tgqpm   1/1     Running             0          2m53s   10.42.5.3   k3d-k3s-default-agent-2    <none>           <none>
fakeshop-5b6b866cf-zlg65   1/1     Running             0          2m52s   10.42.1.4   k3d-k3s-default-server-1   <none>           <none>
postgre-68cbd495c7-vt2k9   1/1     Running             0          9m44s   10.42.3.3   k3d-k3s-default-server-2   <none>           <none>
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo cod~/.kube/config
sudo: cod~/.kube/config: command not found
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo code ~/.kube/config
sudo: code: command not found
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ code ~/.kube/config
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get nodes
NAME                       STATUS   ROLES                       AGE   VERSION
k3d-k3s-default-agent-0    Ready    <none>                      26m   v1.31.5+k3s1
k3d-k3s-default-agent-1    Ready    <none>                      26m   v1.31.5+k3s1
k3d-k3s-default-agent-2    Ready    <none>                      26m   v1.31.5+k3s1
k3d-k3s-default-server-0   Ready    control-plane,etcd,master   27m   v1.31.5+k3s1
k3d-k3s-default-server-1   Ready    control-plane,etcd,master   27m   v1.31.5+k3s1
k3d-k3s-default-server-2   Ready    control-plane,etcd,master   26m   v1.31.5+k3s1
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
NAME                           READY   STATUS    RESTARTS   AGE
pod/fakeshop-5b6b866cf-bsmfq   1/1     Running   0          21m
pod/fakeshop-5b6b866cf-cd7dt   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-chxx5   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-ck7k8   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-h6n55   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-hplw9   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-k5p5v   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-ms68f   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-tgqpm   1/1     Running   0          19m
pod/fakeshop-5b6b866cf-zlg65   1/1     Running   0          19m
pod/postgre-68cbd495c7-vt2k9   1/1     Running   0          26m

NAME                 TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   26m
service/kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          28m
service/postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         26m

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   10/10   10           10          26m
deployment.apps/postgre    1/1     1            1           26m

NAME                                 DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5b6b866cf   10        10        10      26m
replicaset.apps/postgre-68cbd495c7   1         1         1       26m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ code ~/.kube/config
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop unchanged
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get nodes
NAME                       STATUS   ROLES                       AGE   VERSION
k3d-k3s-default-agent-0    Ready    <none>                      29m   v1.31.5+k3s1
k3d-k3s-default-agent-1    Ready    <none>                      29m   v1.31.5+k3s1
k3d-k3s-default-agent-2    Ready    <none>                      29m   v1.31.5+k3s1
k3d-k3s-default-server-0   Ready    control-plane,etcd,master   30m   v1.31.5+k3s1
k3d-k3s-default-server-1   Ready    control-plane,etcd,master   30m   v1.31.5+k3s1
k3d-k3s-default-server-2   Ready    control-plane,etcd,master   29m   v1.31.5+k3s1
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
NAME                           READY   STATUS    RESTARTS   AGE
pod/fakeshop-5b6b866cf-bsmfq   1/1     Running   0          24m
pod/fakeshop-5b6b866cf-cd7dt   1/1     Running   0          21m
pod/fakeshop-5b6b866cf-chxx5   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-ck7k8   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-h6n55   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-hplw9   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-k5p5v   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-ms68f   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-tgqpm   1/1     Running   0          22m
pod/fakeshop-5b6b866cf-zlg65   1/1     Running   0          22m
pod/postgre-68cbd495c7-vt2k9   1/1     Running   0          29m

NAME                 TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   29m
service/kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          30m
service/postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         29m

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   10/10   10           10          29m
deployment.apps/postgre    1/1     1            1           29m

NAME                                 DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5b6b866cf   10        10        10      29m
replicaset.apps/postgre-68cbd495c7   1         1         1       29m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ code ~/.kube/config
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get nodes
NAME                       STATUS   ROLES                       AGE   VERSION
k3d-k3s-default-agent-0    Ready    <none>                      31m   v1.31.5+k3s1
k3d-k3s-default-agent-1    Ready    <none>                      31m   v1.31.5+k3s1
k3d-k3s-default-agent-2    Ready    <none>                      31m   v1.31.5+k3s1
k3d-k3s-default-server-0   Ready    control-plane,etcd,master   32m   v1.31.5+k3s1
k3d-k3s-default-server-1   Ready    control-plane,etcd,master   32m   v1.31.5+k3s1
k3d-k3s-default-server-2   Ready    control-plane,etcd,master   31m   v1.31.5+k3s1
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl config current-context
do-nyc1-aula-k8s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get nodes --context do-nyc1-aula-k8s
NAME                   STATUS   ROLES    AGE   VERSION
pool-ujkvtbn20-676kd   Ready    <none>   14m   v1.32.2
pool-ujkvtbn20-676ki   Ready    <none>   14m   v1.32.2
pool-ujkvtbn20-676kv   Ready    <none>   14m   v1.32.2
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
NAME                           READY   STATUS    RESTARTS   AGE
pod/fakeshop-5b6b866cf-bsmfq   1/1     Running   0          30m
pod/fakeshop-5b6b866cf-cd7dt   1/1     Running   0          27m
pod/fakeshop-5b6b866cf-chxx5   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-ck7k8   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-h6n55   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-hplw9   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-k5p5v   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-ms68f   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-tgqpm   1/1     Running   0          28m
pod/fakeshop-5b6b866cf-zlg65   1/1     Running   0          28m
pod/postgre-68cbd495c7-vt2k9   1/1     Running   0          35m

NAME                 TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.43.66.179   <none>        5000:30000/TCP   35m
service/kubernetes   ClusterIP   10.43.0.1      <none>        443/TCP          36m
service/postgre      ClusterIP   10.43.25.232   <none>        5432/TCP         35m

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   10/10   10           10          35m
deployment.apps/postgre    1/1     1            1           35m

NAME                                 DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5b6b866cf   10        10        10      35m
replicaset.apps/postgre-68cbd495c7   1         1         1       35m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all --context do-nyc1-aula-k8s
Error in configuration: context was not found for specified context: do-nyc1-aula-k8s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ k3d cluster stop k3s-default
ERRO[0000] Failed to get nodes for cluster 'k3s-default': docker failed to get containers with labels 'map[k3d.cluster:k3s-default]': failed to list containers: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.46/containers/json?all=1&filters=%7B%22label%22%3A%7B%22app%3Dk3d%22%3Atrue%2C%22k3d.cluster%3Dk3s-default%22%3Atrue%7D%7D": dial unix /var/run/docker.sock: connect: permission denied
FATA[0000] No nodes found for given cluster
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo k3d cluster stop k3s-default
INFO[0000] Stopping cluster 'k3s-default'
^C
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get nodes
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl get all
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
The connection to the server 0.0.0.0:46589 was refused - did you specify the right host or port?
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get all
NAME                 TYPE        CLUSTER-IP   EXTERNAL-IP   PORT(S)   AGE
service/kubernetes   ClusterIP   10.109.0.1   <none>        443/TCP   20m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get nodes
NAME                   STATUS   ROLES    AGE   VERSION
pool-ujkvtbn20-676kd   Ready    <none>   18m   v1.32.2
pool-ujkvtbn20-676ki   Ready    <none>   18m   v1.32.2
pool-ujkvtbn20-676kv   Ready    <none>   18m   v1.32.2
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
error: error validating "k8s/deployment.yaml": error validating data: failed to download openapi: Get "https://0.0.0.0:46589/openapi/v2?timeout=32s": dial tcp 0.0.0.0:46589: connect: connection refused; if you choose to ignore these errors, turn validation off with --validate=false
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ sudo kubectl apply -f k8s/deployment.yaml
error: error validating "k8s/deployment.yaml": error validating data: failed to download openapi: Get "https://0.0.0.0:46589/openapi/v2?timeout=32s": dial tcp 0.0.0.0:46589: connect: connection refused; if you choose to ignore these errors, turn validation off with --validate=false
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre created
service/postgre created
deployment.apps/fakeshop created
service/fakeshop created
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get nodes
NAME                   STATUS   ROLES    AGE   VERSION
pool-ujkvtbn20-676kd   Ready    <none>   21m   v1.32.2
pool-ujkvtbn20-676ki   Ready    <none>   21m   v1.32.2
pool-ujkvtbn20-676kv   Ready    <none>   21m   v1.32.2
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop unchanged
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get pod
NAME                        READY   STATUS    RESTARTS   AGE
fakeshop-5fd78565c9-2rj9r   1/1     Running   0          2m21s
fakeshop-5fd78565c9-4m425   1/1     Running   0          2m21s
fakeshop-5fd78565c9-8zjbh   1/1     Running   0          2m21s
fakeshop-5fd78565c9-jc948   1/1     Running   0          2m21s
fakeshop-5fd78565c9-lgflr   1/1     Running   0          2m21s
fakeshop-5fd78565c9-pkcgj   1/1     Running   0          2m21s
fakeshop-5fd78565c9-pt8sb   1/1     Running   0          2m21s
fakeshop-5fd78565c9-sngtz   1/1     Running   0          2m21s
fakeshop-5fd78565c9-vsvgd   1/1     Running   0          2m21s
fakeshop-5fd78565c9-zbjp8   1/1     Running   0          2m21s
postgre-8dcf54665-9bwmk     1/1     Running   0          2m21s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get all
NAME                            READY   STATUS    RESTARTS   AGE
pod/fakeshop-5fd78565c9-2rj9r   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-4m425   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-8zjbh   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-jc948   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-lgflr   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-pkcgj   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-pt8sb   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-sngtz   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-vsvgd   1/1     Running   0          2m28s
pod/fakeshop-5fd78565c9-zbjp8   1/1     Running   0          2m28s
pod/postgre-8dcf54665-9bwmk     1/1     Running   0          2m28s

NAME                 TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     NodePort    10.109.12.141   <none>        5000:30000/TCP   2m28s
service/kubernetes   ClusterIP   10.109.0.1      <none>        443/TCP          23m
service/postgre      ClusterIP   10.109.21.238   <none>        5432/TCP         2m29s

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   10/10   10           10          2m29s
deployment.apps/postgre    1/1     1            1           2m29s

NAME                                  DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5fd78565c9   10        10        10      2m29s
replicaset.apps/postgre-8dcf54665     1         1         1       2m29s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop unchanged
service/fakeshop configured
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get all
NAME                            READY   STATUS    RESTARTS   AGE
pod/fakeshop-5fd78565c9-2rj9r   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-4m425   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-8zjbh   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-jc948   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-lgflr   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-pkcgj   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-pt8sb   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-sngtz   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-vsvgd   1/1     Running   0          3m30s
pod/fakeshop-5fd78565c9-zbjp8   1/1     Running   0          3m30s
pod/postgre-8dcf54665-9bwmk     1/1     Running   0          3m30s

NAME                 TYPE           CLUSTER-IP      EXTERNAL-IP   PORT(S)          AGE
service/fakeshop     LoadBalancer   10.109.12.141   <pending>     5000:30000/TCP   3m29s
service/kubernetes   ClusterIP      10.109.0.1      <none>        443/TCP          24m
service/postgre      ClusterIP      10.109.21.238   <none>        5432/TCP         3m30s

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   10/10   10           10          3m31s
deployment.apps/postgre    1/1     1            1           3m31s

NAME                                  DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5fd78565c9   10        10        10      3m31s
replicaset.apps/postgre-8dcf54665     1         1         1       3m31s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get all
NAME                            READY   STATUS    RESTARTS   AGE
pod/fakeshop-5fd78565c9-2rj9r   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-4m425   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-8zjbh   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-jc948   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-lgflr   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-pkcgj   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-pt8sb   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-sngtz   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-vsvgd   1/1     Running   0          7m4s
pod/fakeshop-5fd78565c9-zbjp8   1/1     Running   0          7m4s
pod/postgre-8dcf54665-9bwmk     1/1     Running   0          7m4s

NAME                 TYPE           CLUSTER-IP      EXTERNAL-IP                                      PORT(S)          AGE
service/fakeshop     LoadBalancer   10.109.12.141   138.197.231.105,2604:a880:400:d1:0:1:47ad:a001   5000:30000/TCP   7m4s
service/kubernetes   ClusterIP      10.109.0.1      <none>                                           443/TCP          28m
service/postgre      ClusterIP      10.109.21.238   <none>                                           5432/TCP         7m5s

NAME                       READY   UP-TO-DATE   AVAILABLE   AGE
deployment.apps/fakeshop   10/10   10           10          7m5s
deployment.apps/postgre    1/1     1            1           7m5s

NAME                                  DESIRED   CURRENT   READY   AGE
replicaset.apps/fakeshop-5fd78565c9   10        10        10      7m5s
replicaset.apps/postgre-8dcf54665     1         1         1       7m5s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop unchanged
service/fakeshop configured
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ cd src
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ docker build -t b3rnar0p/fake-shop-desafio:v2 .
ERROR: permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Head "http://%2Fvar%2Frun%2Fdocker.sock/_ping": dial unix /var/run/docker.sock: connect: permission denied
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo docker build -t b3rnar0p/fake-shop-desafio:v2 .
[+] Building 4.4s (13/13) FINISHED                                                                       docker:default
 => [internal] load build definition from Dockerfile                                                               0.0s
 => => transferring dockerfile: 293B                                                                               0.0s
 => [internal] load metadata for docker.io/library/python:3.11.0                                                   1.7s
 => [auth] library/python:pull token for registry-1.docker.io                                                      0.0s
 => [internal] load .dockerignore                                                                                  0.1s
 => => transferring context: 2B                                                                                    0.0s
 => [1/7] FROM docker.io/library/python:3.11.0@sha256:55101c8373de5311b0ece8746251882ddb0bb394588c93d2477b88852ad  0.0s
 => [internal] load build context                                                                                  0.9s
 => => transferring context: 11.06kB                                                                               0.9s
 => CACHED [2/7] COPY requirements.txt .                                                                           0.0s
 => CACHED [3/7] RUN python -m pip install -r requirements.txt                                                     0.0s
 => CACHED [4/7] WORKDIR /app                                                                                      0.0s
 => [5/7] COPY . /app                                                                                              0.2s
 => [6/7] RUN chmod +x /app/entrypoint.sh                                                                          0.6s
 => [7/7] RUN mkdir -p /tmp/metrics                                                                                0.4s
 => exporting to image                                                                                             0.3s
 => => exporting layers                                                                                            0.2s
 => => writing image sha256:1ec27f4564a184ed7447cb58117a7e87644ab6e68a93a3413953a70fe8dc08c0                       0.0s
 => => naming to docker.io/b3rnar0p/fake-shop-desafio:v2                                                           0.0s
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo docker push /b3rnar0p/fake-shop-desafio:v2
invalid reference format
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo docker push b3rnar0p/fake-shop-desafio:v2
The push refers to repository [docker.io/b3rnar0p/fake-shop-desafio]
f5f7cdb3262b: Pushed
c305912c22d8: Pushed
8fb5321a3af8: Pushed
42a7de8ccf63: Layer already exists
a2b78eed1422: Layer already exists
54c8b000e46c: Layer already exists
0cd2264d51c3: Layer already exists
02bfc2ce10fa: Layer already exists
e35157207868: Layer already exists
1cad4dc57058: Layer already exists
4ff8844d474a: Layer already exists
b77487480ddb: Layer already exists
cd247c0fb37b: Layer already exists
cfdd5c3bd77e: Layer already exists
870a241bfebd: Layer already exists
v2: digest: sha256:6e27c3653236f04eeed728869d77cc6d732aeff88c671f0afeff5fea8ba30a86 size: 3467
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ kubectl apply -f k8s/deployment.yaml
error: the path "k8s/deployment.yaml" does not exist
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ asudo kubectl apply -f k8s/deployment.yaml
Command 'asudo' not found, did you mean:
  command 'sudo' from deb sudo (1.9.14p2-1ubuntu1)
  command 'sudo' from deb sudo-ldap (1.9.14p2-1ubuntu1)
Try: sudo apt install <deb name>
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ sudo kubectl apply -f k8s/deployment.yaml
error: the path "k8s/deployment.yaml" does not exist
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop/src$ cd ..
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop configured
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop configured
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl apply -f k8s/deployment.yaml && watch 'kubectl get po'
deployment.apps/postgre unchanged
service/postgre unchanged
deployment.apps/fakeshop configured
service/fakeshop unchanged
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl get replicaset
NAME                  DESIRED   CURRENT   READY   AGE
fakeshop-558c84645d   10        10        10      3m26s
fakeshop-5fd78565c9   0         0         0       19m
postgre-8dcf54665     1         1         1       19m
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl rollout history deployment fakeshop
deployment.apps/fakeshop
REVISION  CHANGE-CAUSE
3         <none>
4         <none>

b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$ kubectl rollout undo deployment fakeshop && watch 'kubectl get po'
deployment.apps/fakeshop rolled back
b3rnard0p@DESKTOP-MFEP8L6:/mnt/c/Users/Win10/fake-shop$
