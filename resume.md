## Comandos

### GIT INIT 

- cria um repositório vazio ou reinicializa um existente, é criada um diretório 
invisível (.git) na pasta onde ele foi inicializado com os arquivos necessários 
para funcionar corretamente. Caso um repositório já exista e rode o comando init 
nenhum problema será gerado, o repositório será apenas reinicializado.

- podemos iniciar o repositório junto com a criação de uma branch com o comando 
'git init -b nome-branch ou 'git init --initial-branch nome-branch'.

* git init
* git init -b (branch-name)
* git init --initial-branch (branch-name)

### GIT ADD 

- adiciona o arquivo no index da pasta (.git), todos os arquivos são armazenados 
num arquivo chamado 'index', caso o arquivo já exista e esteja adicionando 
novamente, ele irá atualizar o arquivo.

- a adição dos arquivos é uma preparação para o próximo commit, portanto ela 
é feita antes do commit. Sempre que um arquivo é criado ou modificado, o git add 
deve ser executado.

* git add (file-name)
* git add .
* git add -a
* git add --all

### GIT BRANCH

- cria, lista ou deleta branchs, usando 'git branch --list' ou apenas 'git branch' 
é lista as branchs existentes no repositório.

* git branch (branch-name) (cria uma branch)
* git branch ou git branch --list (lista as branchs)
* git branch -M (new-name) (renomeia a branch)
* git branch -D (branch-name) (deleta a branch, não pode estar nela ao deletar)

### GIT COMMIT

- salva as mudanças no repositório. Deve-se também passar uma mensagem como 
argumento descrevendo a mudança que foi realizada naquele ponto específico.
Sempre antes de executar um commit, deve-se executar o git add para adicionar 
as mudanças no repositório.

- para nao usar dois comandos sempre, podemos usar o comando abaixo para adicionar 
e comitarmos as modificações ao mesmo tempo.

* git commit -a -m "mensagem" (adiciona e comita arquivos modificados e deletados)

### GIT RM (ARQUIVO)

- exclui o arquivo e remove do monitoramente do git

### GIT MV (ARQUIVO / DESTINO)

- move o arquivo de um local para outro
- no momento do argumento de destino, pode-se passar com outro nome
- assim o arquivo será movido e renomeado ao mesmo tempo

* git mv ./css/file1.md ./dist/file1.md (movendo arquivo)
* git mv ./css/file1.md ./dist/file-new.md (movendo e renomeando)

https://git-scm.com/docs/git-commit