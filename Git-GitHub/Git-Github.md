# Git

Aplicação para versionamento de softwares.  
Download: https://git-scm.com/downloads

## Git Bash

O Git Bash é um CLI, que acompanha a instalação do Git, utilizado de forma a otimizar o uso de comandos git.

## Git Hub

O Github é uma plataforma de hospedagem remota de repositórios com forte viés em trabalho colaborativo.

## Principais comandos:

- `git init`: Inicia o versionamento no diretório
- `git add <nome do arquivo>`: Adiciona o arquivo em questão à área de staging
- `git commit -m "<mensagem>"`: Cria nova versão do projeto atualizando todos os itens na área de staging
- `git remote add origin <url do repositorio>`: Cria link para repositório remoto (Github)
- `git pull origin master`: Puxa o commit do repositório remoto para o repositório de trabalho
- `git push origin master`: Sobe o commit do repositório local para o remoto
- `git clone <url>`: Clona o repositório indicado para diretório atual