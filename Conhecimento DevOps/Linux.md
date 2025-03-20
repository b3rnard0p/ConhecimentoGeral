# 🐧 Linux

**Linux** é um sistema operacional de código aberto baseado no núcleo (kernel) Linux. Ele é amplamente utilizado em servidores, computadores pessoais, dispositivos embarcados e sistemas de supercomputação. Diferente de sistemas proprietários como Windows e macOS, o Linux é distribuído sob a licença **GPL (General Public License)**, permitindo que qualquer pessoa possa usar, modificar e distribuir o sistema gratuitamente.

O Linux é conhecido por sua **estabilidade**, **segurança** e **eficiência**, sendo o sistema operacional de escolha para a maioria dos servidores web e serviços em nuvem. Existem várias distribuições (ou "distros") de Linux, como **Ubuntu**, **Debian**, **Fedora**, **CentOS**, **Arch Linux**, entre outras, cada uma com características específicas.

## ⚙️ Características do Linux

- **Código aberto e gratuito**.
- **Sistema multitarefa e multiusuário**.
- **Alta estabilidade e segurança**.
- **Altamente personalizável**.
- **Grande variedade de distribuições** para diferentes finalidades.
- **Ampla comunidade de suporte e documentação disponível**.

## 💻 Comandos Básicos do Terminal Linux

Aqui estão alguns dos comandos mais comuns para começar a usar o terminal do Linux:

### 📂 Navegação entre diretórios

```
pwd          # Exibe o diretório atual
ls           # Lista os arquivos e diretórios do diretório atual
ls -la       # Lista detalhada incluindo arquivos ocultos
cd /caminho  # Muda para o diretório especificado
cd ..        # Volta um diretório
cd ~         # Vai para o diretório home do usuário
```

### 📄 Gerenciamento de arquivos e diretórios
```
touch arquivo.txt        # Cria um novo arquivo vazio
mkdir pasta              # Cria um novo diretório
cp origem destino        # Copia arquivos ou diretórios
mv origem destino        # Move ou renomeia arquivos ou diretórios
rm arquivo.txt           # Remove um arquivo
rm -r pasta              # Remove um diretório e seu conteúdo
```

### 🔍 Visualização e manipulação de arquivos
```
cat arquivo.txt          # Exibe o conteúdo de um arquivo
less arquivo.txt         # Exibe o conteúdo com paginação
head arquivo.txt         # Exibe as 10 primeiras linhas
tail arquivo.txt         # Exibe as 10 últimas linhas
nano arquivo.txt         # Edita o arquivo usando o editor nano
```

### 🔑 Permissões e usuários
```
chmod 755 arquivo.sh     # Altera as permissões do arquivo
chown user:grupo arquivo # Altera o proprietário do arquivo
whoami                   # Mostra o usuário atual
sudo comando             # Executa um comando como superusuário
```

### 🔄 Atualização e instalação de pacotes (Debian/Ubuntu)
```
sudo apt update                # Atualiza a lista de pacotes disponíveis
sudo apt upgrade               # Atualiza os pacotes instalados
sudo apt install nome_pacote   # Instala um pacote
sudo apt remove nome_pacote    # Remove um pacote
```
### 📊 Informações do sistema
```
uname -a               # Mostra informações do kernel
df -h                  # Mostra o uso de disco
free -h                # Mostra o uso de memória RAM
top                    # Exibe processos em execução em tempo real
```

# 🚀 WSL

O **WSL (Windows Subsystem for Linux)** é uma camada de compatibilidade desenvolvida pela Microsoft que permite aos usuários **executar distribuições Linux** nativas diretamente no Windows, sem a necessidade de uma máquina virtual ou dual boot. O WSL fornece uma experiência de **sistema Linux completo** em ambientes Windows, permitindo que desenvolvedores aproveitem as ferramentas, utilitários e softwares do Linux sem precisar sair do ecossistema Windows.

## 🏗️ Características do WSL

- **Compatibilidade Total com o Linux**: Com o WSL, você pode rodar **distros Linux** completas, como Ubuntu, Debian, Fedora, e muitas outras, diretamente no Windows.
- **Integração entre Linux e Windows**: O WSL permite que você **execute comandos do Linux** e utilize ferramentas nativas do Windows ao mesmo tempo, facilitando a troca de arquivos e integração entre os dois sistemas.
- **Desempenho**: O WSL, especialmente o **WSL 2**, foi otimizado para oferecer uma **performance quase nativa**, permitindo que você utilize a linha de comando do Linux de maneira muito eficiente dentro do Windows.
- **Acesso a Ferramentas de Desenvolvimento**: É possível usar ferramentas populares de desenvolvimento do Linux, como **git, node.js, python, Docker, entre outras**, diretamente no Windows.
- **Sem necessidade de máquinas virtuais**: O WSL permite executar o Linux sem precisar de uma máquina virtual, economizando recursos e proporcionando maior velocidade de execução.

## 🔄 WSL 1 vs WSL 2

O **WSL 1** foi a primeira versão, permitindo rodar um kernel Linux compatível com o sistema Windows, mas com algumas limitações de desempenho e compatibilidade. Já o **WSL 2** trouxe uma grande melhoria, passando a utilizar um **kernel Linux completo**, com suporte completo para sistemas de arquivos, permitindo uma integração mais eficiente entre o Windows e o Linux, com **maior desempenho** e **compatibilidade melhorada**.

### **Principais diferenças:**
- **WSL 1** usa um sistema de tradução de chamadas de sistema, o que pode resultar em algumas limitações de performance e compatibilidade.
- **WSL 2** usa um kernel completo do Linux, o que melhora o suporte a contêineres e a execução de aplicativos nativos de Linux, além de melhorar o desempenho do sistema de arquivos.

## 🔄 Como Funciona o WSL?

1️⃣ **Instalação**: O WSL pode ser instalado diretamente do **PowerShell** ou da **Microsoft Store**. Você pode escolher qual distribuição do Linux deseja usar, como **Ubuntu, Debian, Kali Linux**, etc.

2️⃣ **Execução**: Depois de instalado, você pode **abrir o terminal do Linux** diretamente dentro do Windows. As distribuições do Linux podem ser iniciadas com simples comandos no prompt de comando ou no PowerShell.

3️⃣ **Interação com o Sistema de Arquivos**: O WSL permite acessar **arquivos do Linux e do Windows** diretamente do terminal. É possível navegar pelo sistema de arquivos do Windows (`/mnt/c/`) e pelo sistema de arquivos do Linux simultaneamente.

4️⃣ **Uso de Ferramentas de Linux**: Você pode instalar e usar ferramentas nativas de Linux, como **compiladores, bibliotecas e frameworks**, diretamente no seu ambiente Windows, sem a necessidade de usar uma máquina virtual.

## 📊 Vantagens do WSL

✅ **Desenvolvimento simplificado**: Com o WSL, você pode aproveitar as ferramentas do Linux, como **Git**, **Docker**, **Python**, etc., sem sair do Windows, tornando o desenvolvimento mais ágil.  
✅ **Integração perfeita**: Permite a interação entre o sistema de arquivos do Windows e o Linux, tornando fácil compartilhar arquivos e executar tarefas que dependem de ambos os sistemas.  
✅ **Maior desempenho**: O WSL 2 oferece uma performance significativamente melhorada em comparação com o WSL 1, principalmente em tarefas de IO e execução de contêineres.  
✅ **Sem necessidade de dual boot ou VM**: Não é necessário reiniciar o computador ou configurar máquinas virtuais pesadas para usar o Linux.

## ❌ Desvantagens do WSL

❌ **Compatibilidade limitada**: Apesar do WSL 2 ter melhorado muito a compatibilidade com o Linux, ainda pode haver limitações em alguns casos, como o suporte a certos módulos ou aplicativos de hardware.  
❌ **Requer versão recente do Windows**: Para utilizar o WSL 2, você precisa estar rodando uma versão mais recente do Windows 10 ou 11, com suporte para virtualização habilitada.  
❌ **Não é 100% equivalente ao Linux nativo**: Mesmo com o WSL 2, o ambiente não é exatamente igual a um sistema Linux completo, o que pode apresentar algumas limitações em termos de desempenho ou comportamento.
