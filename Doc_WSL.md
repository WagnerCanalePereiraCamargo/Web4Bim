
# Iniciando a Configuração do Ambiente de Desenvolvimento atraves da WSL

## Índice
1. [Habilitar o WSL e a Plataforma de Máquina Virtual](#1---habilitar-o-wsl-e-a-plataforma-de-máquina-virtual)
2. [Baixar o Pacote de Atualização do Kernel do Linux](#2---baixar-o-pacote-de-atualização-do-kernel-do-linux)
3. [Instalar o Ubuntu](#3---instalar-o-ubuntu)
4. [Iniciando a Virtualização](#4---iniciando-a-virtualização)
5. [Importar e Exportar Distribuições](#5---importar-e-exportar-distribuições)
6. [Encerrando a Virtualização](#6---encerrando-a-virtualização)

---

## 1 - Habilitar o WSL e a Plataforma de Máquina Virtual

Para utilizar o Windows Subsystem for Linux (WSL), é necessário habilitar o subsistema Linux e a plataforma de máquina virtual. Abra o PowerShell como administrador e execute os comandos abaixo:

```powershell
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

Esses comandos habilitam os recursos necessários para rodar o WSL.

---

## 2 - Baixar o Pacote de Atualização do Kernel do Linux

Agora, vamos instalar e atualizar o kernel do Linux para o WSL.

- Para instalar o WSL e atualizar o kernel, execute:

  ```bash
  wsl.exe --install
  wsl.exe --update
  ```

- Em seguida, defina o WSL 2 como a versão padrão com o comando:

  ```bash
  wsl --set-default-version 2
  ```

- Para acessar as configurações dos recursos do Windows (caso queira ativá-los manualmente):

  ```bash
  control appwiz.cpl
  ```

---

## 3 - Instalar o Ubuntu

Para verificar as distribuições de Linux disponíveis e confirmar se o Ubuntu está instalado, use:

```bash
wsl -l -v
```

Se o Ubuntu não estiver instalado, liste as distribuições disponíveis para instalar:

```bash
wsl.exe --list --online
```

Escolha uma distribuição da lista e instale-a com o comando:

```bash
wsl.exe --install <Distro>
```

Após a instalação, reinicie o computador e, ao iniciar o WSL novamente, você será solicitado a criar um nome de usuário e senha para o ambiente Linux.

---

## 4 - Iniciando a Virtualização

Para iniciar a virtualização com a distribuição instalada (no caso, Ubuntu), execute:

```bash
wsl -d Ubuntu -u <nome_usuario>
```

### Executar Scripts para Configuração

Para atualizar o sistema com um script, use o comando `curl` para baixar o arquivo:

```bash
curl -O <URL do script em formato Raw>
```

Depois, altere as permissões do script para torná-lo executável:

```bash
sudo chmod +x ./setup_sources.sh
```

Para executar o script:

```bash
./setup_sources.sh
```

> **Dica**: Você pode repetir esses mesmos comandos para instalar o Visual Studio Code. Com o comando `code .`, o VS Code será iniciado dentro do ambiente virtualizado.

---

## 5 - Importar e Exportar Distribuições

### Importar uma Distribuição

Se desejar importar uma máquina WSL previamente exportada, utilize o comando abaixo, substituindo os parâmetros conforme necessário:

```bash
wsl --import <nome-nova-maquina> <caminho-para-salvar> <caminho-do-arquivo-exportado>
```

**Exemplo**:

```bash
wsl --import contatica a:\wsl\contatica a:\wsl\template.tar
```

### Exportar uma Distribuição

Para exportar uma máquina WSL existente, execute:

```bash
wsl --export <Nome-da-Distribuição> <caminho-de-destino/nome-arquivo.tar>
```

**Exemplo**:

```bash
wsl --export Ubuntu c:\wsl\template.tar
```

---

## 6 - Encerrando a Virtualização

Para sair da sessão do WSL, utilize o comando:

```bash
exit
```

Para encerrar completamente a virtualização do WSL, use:

```bash
wsl --shutdown
```

---

Esse guia cobre as etapas principais para configurar e gerenciar o ambiente WSL no Windows.