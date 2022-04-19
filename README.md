# N1 Glauco

Equipe: Gustavo Bosco, Wilson Marutti e Frederico Bernardes Wust Stein.

Nesse readme contém um tutorial sobre o uso do GIT

1.Como inicializar repositórios:

Para iniciar repositórios via GIT, é utilizado o comando “git init”. Assim, terá um lugar para gravar as alterações do projeto.


2.Como fazer o primeiro commit em um projeto:

Para fazer o primeiro commit em um projeto, é utilizado o comando “git add” para incluir atualizações a um arquivo específico no próximo commit. Não ocorrerá um efeito real no repositório, mas assim será possível gravar mudanças na próxima execução.


3.Como realizar commit de mudanças:

Para fazer o commit de mudanças, em um projeto, é utilizado o comando “git commit -m “” ”, onde a alteração no projeto será salva no repositório, podendo acrescentar também uma mensagem ao commit, dentro das aspas.


4.Como compartilhar suas mudanças com outras pessoas da equipe:

Para compartilhar as mudanças com outras equipes, deve-se criar um meio de comunicação entre as equipes. Para isso, o comando “git push” empurra o repositório local para o repositório online. No caso de uma primeira vez utilizando o “git push”, deve-se criar uma “branch master” no repositório online através do comando “git  push -u origin master, sendo assim, as demais equipes poderão compartilhar suas mudanças dentro da branch master.


5.Como desfazer alterações:

Para se desfazer das alterações, é utilizado o comando “git revert”, assim ele manterá commits que você deseja desfazer e criará um novo commit que inverte o commit indesejado.


6.Como resolver conflitos de merge:

Caso você queira se desfazer de alterações em um arquivo específico que esteja ocasionando em conflito, é utilizado o comando “git reset” para descartar essas alterações locais.


7.Como usar branches:

Para utilizar branches, basta executar o comando “git branch” para visualizar todas as branches disponíveis e executar “git checkout nomeDaBranch” para abri-la. Caso não exista uma branch, é executado o comando “git branch nomeDaNovaBranch” para criar uma.


8.Como encontrar bugs (git diff, git log, git bisect, git blame):

Git bisect: Para encontrar bugs com git bisect, é executado primeiramente o “git bisect start” para começar a busca do bug, depois, o “git bisecat bad” para informar ao Git buscar por erros/bugs. Caso você souber de alguma versão dentre seu repositório que não tenha problemas, você pode informar ao git com “git bisect good nomeDaSuaBranch, para ele aplicar uma contagem binária entre as versões do repositório, auxiliando ao usuário para testar alguma específica versão onde possa estar a versão com bug.

Git diff: Para realizar comparações de alterações com o comando “git diff”, basta executá-lo que ele realiza uma função de comparação nas fontes de dados do Git, onde elas são commits, ramificações, arquivos e outros. E claro, executar o comando na sua branch desejada.

Git log: Com o comando “git log”, é possível visualizar o desenvolvimento de uma determinada branch. Esse comando visualiza o histórico de alterações, mostrando os nomes de cada branch commitada.

Git blame: O comando “git blame” serve para examinar o conteúdo linha por linha de um arquivo. Podendo saber quando cada linha foi modificada pela última vez e quem foi o autor da mudança. Sendo assim, você pode dar um “git clone” de algum algum repositório como exemplo e em seguida executar o “git blame” para ver o histórico do repositório.


9.Como escolher determinados commits utilizando o comando "git cherry pick": 

Em caso de dois usuários encontrarem um problema que atinge ambos, mesmo em branches diferentes, e um deles fazer a correção, você não pode fazer o merge, você precisará da correção. É nesse momento que utilizamos o "git cherry pick", onde é possível pegar um commit e copiá-lo de uma branch para outra. Para isso, deve-se pegar o identificador da branch corrigida(esse identificador é um ID da sua branch, com misturas sequencial de números e letras), para copiá-la a sua branch. Seria nesse sentido: "git checkout nomeBranchCorrigida", depois utilize execute o "git log" para encontrar o ID do commit e copiá-la, e assim, volte para sua branch e execute "git cherry pick idBranch". 
