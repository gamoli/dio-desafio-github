# Chave SSH

### Como criar e habilitar o par de chaves SSH para utilização no GitHub

#### No Git Bash

1. Gerar par de chaves SSH: ``ssh-keygen -t ed -C <email>``
2. Ignorar a mudança de caminho do arquivo: Aperte "Enter"
3. Digitar senha para uso da chave: digite uma senha ou apenas aperte "Enter" para ignorar o passo
4. Confirmar senha: digite novamente a senha ou aperte "Enter" para ignorar
5. Mudar para o diretório da chave SSH: ``cd /c/Users/<nome_usuario>/.ssh/``
6. Inicializar o agente SSH: ``eval $(ssh-agent -s)``
7. Entrega chava privada ao agente: ``ssh-add id_ed25519``
8. Insere a senha da chave: caso não haja, aperte "Enter"
9. Exibir dados da chave pública: ``cat id_ed.pub``
10. Extrair chave: selecione e copie os dados exibidos no terminal após o último passo

#### No GitHub

11. Abrir a página de configurações de perfil do usuário: [settings](https://github.com/settings/profile)
12. Ir para "SSH and GPG keys"
13. Clicar em "New SSH key"
14. Dar um nome à chave no campo "Title"
15. Colar os dados da chave pública (copiados no passo 10) no campo "key"
16. Clicar em "Add SSH key"
17. Autenticar-se