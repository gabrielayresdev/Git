# Git

## Definições

### Repositório 
Um repositório contém todos os arquivos do seu projeto e o histórico de revisão de cada arquivo. Você pode discutir e gerenciar o trabalho do projeto dentro do repositório.

### Commit
Os commits são as unidades estruturais de um cronograma de projeto Git. Podem ser considerados instantâneos ou marcos ao longo do cronograma de um projeto Git.

### .gitignore
Arquivo onde são informados os arquivos/pastas que não serão monitoradas pelo git. Nele devem ser escritos os nomes de cada arquivo ou pasta que serão ignoradas.
 
### Branch
Uma ramificação no git é um ponteiro para as alterações feitas nos arquivos do projeto. É útil em situações nas quais você deseja adicionar um novo recurso ou corrigir um erro, gerando uma nova ramificação garantindo que o código instável não seja mesclado nos arquivos do projeto principal.

## Comandos

### git init
Inicializa um repositório na pasta selecionada. Desse modo, toda alteração no repositório é monitorada.

### git status 
Apresenta informações sobre o status do repositório.

### git add
Seleciona um arquivo para fazer o commit.

### git commit -m ""
Realiza um commit e adiciona com a mensagem que estiver dentro das aspas.

### git log
Apresenta um histórico informando os commits feitos no repositório, seus hashs, branch, autor, data, hora e mensagem. Um variante do comando é o git log -p, onde mais informações serão exibidas. Outra variante é o git log --oneline, onde menos informações serão exibidas. O site https://devhints.io/git-log-format pode ser consultado para mais informações sobre a formatação do git log.

### git config --local user.name ""
Define um nome para o autor dos commits do projeto atual. --local pode ser substituido por --global para que sejam definido um nome para todos os projetos.

### git config --local user.email ""
Define um email para o autor dos commits do projeto atual. --local pode ser substituido por --global para que sejam definido um email para todos os projetos.

### git init --bare
Inicia um repositório pushable. Geralmente é usado no servidor e informa que o repositório será usado apenas para armazenas as modificações.

### git remote
Lista todos os repositórios remotos que o projeto possui.

### git remote rename [nome original] [nome novo]
Renomeia um repositório remoto.

### git remote add [nome] [endereço]
Adiciona um repositório remoto ao projeto.

### git clone [endereço] [nome]
Faz a cópia dos arquivos armazenados no servidor.

### git push [repositório remoto] [branch]
Envia os arquivos do repositório para o servidor.

### git pull [repositório remoto] [branch]
Baixa os arquivos do servidor para o repositório.

### git branch 
Exibe todos os branches existentes.

### git branch [nome]
Cria um novo branch.

### git checkout [branch]
Seleciona o branch que irá realizar os commits.

### git checkout -b [nome]
Cria e seleciona o branch que irá realizar os commits.

### git merge [branch]
Une as alterações da branch chamada a branch atual.

### git rebase [branch]
Funciona de modo semelhante ao git merge, porém não realiza um commit de merge. 

## Boas práticas

### Quando não realizar um commit
Nunca se deve commitar um código que não funciona.
