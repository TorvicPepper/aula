instalar o git

git init
transforma o repositorio em repositorio git

git add .
adiciona todos os arquivos para o git

git config --global user.email "exemplo"
adiciona o email q esta usando no github

git config --global user.user "exemplo"
adiciona o usuario q esta usando no github

git commit -m "first commit"
registra os arquivos no repositorio

git branch -M main

git remote add origin git@github.com:nomeusuario/repositorio.git
faz o link com o github

	é necessario autenticação
	gerar chave ssh
	github>settings>ssh and gpg keys > nova chave ssh.
	fica salvo na pasta
	pasta pessoal> pasta oculta .ssh
	no terminal ssh-keygen -t ed25519 -C "emailgithub"
	vai criar a chave no .ssh
	abra a chave publica copia e cola no site do github no ssh and gpg keys

git push -u origin main
faz a conexão

git remote -v
Listar os repositórios remotos

git remote add apelido url
Adicionar um repositório remoto

git remote remove origin
Remover um repositório remoto

git remote set-url origin https://github.com/seu-usuario/seu-repositorio.git
Alterar a URL de um repositório remoto

git remote rename origin novo-origin
 Alterar o apelido de um repositório remoto

clonando un repositorio
git clone url

git status
mostra as mudanças 

git add .
git commit "alterando"
vai alterar os arquivos o comiit serve para crar versão 

git log 
historico dos commits

git remote origin
git push origin main
envia os commits para o repositorio no github
	se for outra pessoa fazendo é necessario permissão de coloborador

se o codigo ta antigo e quer puxar do github

git pull origin
puxa os commits do github

git status: verificar quais arquivos foram modificados
git add: adicionar mudanças
git commit: registrar as mudanças no repositorio
git push: subir as mudanças para o repositorio
git pull: baixar as mudanças para o repositorio local

reverter commit
	git log
	git revert id

apagando commit
	git log
	git reset --hard id
	--hard apaga o commit e e desfaz
	cuidado só no local

alterar mensagem do commit
	git log
	git commit --amend -m "mensagem"
	altera o commit anterior

ignorar arquivos ou repositorios
	n usar git add. pois adiciona tudo
	.gitignore crie o arquivo e coloque oq quer ignorar
	gitingone.io site q cria um template do oque ignorar
