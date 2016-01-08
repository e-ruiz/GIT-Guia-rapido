# Git-Quick-Reference
A short GIT referece to survive on development

**Compilado do guia:**
https://training.github.com/kit/downloads/pt/github-git-cheat-sheet.pdf

**OBS.:** esse guia está incompleto, acesse o link acima para ver a versão completa.


## Instale o GIT

GitHub fornece clientes desktop que incluem uma interface gráfica para as ações mais comuns em um  repositório e atualiza automaticamente para a linha de comando do Git para cenários avançados.

**GitHub para Windows:** https://windows.github.com

**GitHub para Mac:** https://mac.github.com

Distribuições do Git para Linux e sistemas POSIX são disponíveis no site oficial do Git SCM.

**Git para todas plataformas:** http://git-scm.com


## Configure a Ferramenta

Com o parâmetro ```--global```, você configura informações de usuário para todos os repositórios locais.

Configura o nome que você quer ligado as suas transações de commit.
```bash
$ git config --global user.name 
```

Configura o email que você quer ligado as suas transações de commit
```bash
$ git config --global user.email "endereco-de-email"
```

Configura apresentação colorida
```bash
$ git config --global color.ui auto
```


## Crie Repositórios
Inicie um novo repositório ou obtenha de uma URL existente.

Cria um novo repositório local com um nome específico:
```bash
$ git init [nome-do-projeto]
```

Baixa um projeto e seu histórico de versão inteiro:
```bash
$ git clone [url]
```


## Faça Mudanças
Revise edições e crie uma transação de commit.

Lista todos os arquivos novos ou modificados para serem commitados
```bash
$ git status
```

Faz o snapshot de um arquivo na preparação para versionamento
```bash
$ git add [arquivo]
```

Deseleciona o arquivo, mas preserva seu conteúdo
```bash
$ git reset [arquivo]
```

Mostra diferenças no arquivo que não foram realizadas
```bash
$ git diff
```

Mostra a diferença entre arquivos selecionados e a suas últimas versões
```bash
$ git diff --staged
```

Grava o snapshot permanentemente do arquivo no histórico de versão
```bash
$ git commit -m "mensagem descritiva"
```


## Mudanças em Grupo
Nomeie uma série de commits e combine os esforços completos.

Lista todos os branches locais no repositório atual
```bash
$ git branch
```

Cria um novo branch
```bash
$ git branch [nome-do-branch]
```

Muda para o branch específico e atualiza o diretório de trabalho
```bash
$ git checkout [nome-do-branch]
```

Combina o histórico do branch específico com o branch atual
```bash
$ git merge [branch]
```

Exclui o branch específico
```bash
$ git branch -d [nome-do-branch]
```
