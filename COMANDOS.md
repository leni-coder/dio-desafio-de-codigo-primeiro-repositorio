#17 comandos Git 

1. Git init: criando repositório local!
O git init serve para criar um repositório localmente, no seu computador. Para criar um novo repositório, cria-se uma pasta (ou se quiser iniciar um repositório em uma pasta que já existe, vá até ela) e digite o comando git init e pronto, o repositório Git foi criado! 

2. Git add: adicionando alterações no repositório!
Quando se cria ou modifica arquivos, precisa-se adicionar eles para a área de staging, para isso usa-se o comando git add* para adicionar todos os arquivos ou git add<nome-do-arquivo>. Dessa forma, os arquivos estarão prontos para serem commitados.

3. Git commit: confirmando e salvando as alterações no repositórios!
Após usar o git add, os arquivos vão para a área de commit. pode-se empacotar todas essas alterações em um único commit com uma mensagem que resume aquelas alterações. Para isso utiliza-se o comando git commit -m “Mensagem das alterações”.

4. Git Status: verificando se há alterações na branch
O git status mostra o status do repositório naquele momento. Ele mostra o working directory, a staging area com todos os arquivos em cada uma das áreas e qual o estado de cada um deles. Isso ajuda muito quando precisamos pensar em fazer um commit ou até mesmo verificar quais foram todos os arquivos modificados.  

5. Git log: verifique quais commits foram feitos até agora
O git log ajuda a saber quais foram os commits feitos no repositório, quem fez, quando e também qual a mensagem de cada um. Além disso, esse comando mostra a hash de cada um dos commits, o que pode ajudar a executar alguns outros comandos também. 

6. Git reset: desfazendo as alterações de um repositório para um commit anterior!
O git reset é uma forma bem complexa para desfazer alterações. 

git reset <hash do commit que se quer voltar>

Após rodar esse comando, o último commit some e as alterações voltaram para o working directory. 

exemplo:
git reset --hard origin/main


7. Git revert: Desfazendo um commit sem excluir os dados existentes!
O git revert faz parte de comandos do tipo “desfazer”. Mas ele não é uma opção tão tradicional. Basicamente, ele cria um novo commit desfazendo o commit que se especificar.

8. Git diff: verificando as diferenças entre arquivos e repositórios!
pode-se ver as diferenças dos arquivos ou também entre os repositórios local e remoto. Para isso, basta rodar o comando git diff depois das alterações feitas no repositório local ou, se precisar ver antes de um merge, por exemplo, também pode executar git diff <branch origem> <branch destino>.

9. Git remote: ligando o repositório local a um repositório remoto!
Se não clonou um repositório, pode ligar o repositório local a um servidor com o comando remote. Para isso, basta usar git remote add origin <servidor>.

10. Git push: enviando as alterações do repositório local para o repositório remoto!
Depois das alterações feitas, adicionadas para a área de staging,dos commits, pode-se fazer o push. Ou seja, se consegue mandar todas essas alterações do repositório local para um remoto. Para isso, usa-se o comando git push origin main, no qual main pode ser substituúida por qualquer outra branch que você estiver trabalhando. 

11. Git branch: listando e deletando branches 
Para listar todas as branches que estão em um repositório, basta rodar git branch. Para deletar uma branch específica basta rodar git branch -d nome_da_branch.

12. Git checkout: criando uma nova branch restaurando arquivos!
Para criar uma nova branch, deve-se rodar o comando git checkout -b nome_da_branch. E, para alternar entre branches, basta rodar git checkout nome_da_branch.

Agora, se tiver feito algo errado e quiser restaurar o arquivo ao seu estado original, pode-se rodar git checkout — nome_do_arquivo. Mas, isso só funcionará se o arquivo ainda estiver no working directory. Caso já esteja na área de staging, terá que, primeiro, fazer um reset para depois conseguir fazer um checkout.

13. Git merge: mesclando as alterações em sua branch à branch master
Quando precisar trazer as atualizações da branch main, a principal, para a branch que está trabalhando, basta rodar da sua branch: git branch main. Se não tiver nenhum conflito nos arquivos que atualizou na sua branch com as alterações da main, não terá que fazer mais nada. Agora se tiver algum conflito, vai aparecer no terminal que houve um conflito e quais os arquivos conflitantes. Precisará abrir cada um deles e escolher qual versão do código vai querer manter. 

14. Git pull: atualizando o repositório local com a versão do repositório remoto! 
Quando precisar atualizar o repositório local com a mais nova versão do repositório remoto, basta usar o comando git pull. Dessa forma, ele verificará se tem uma versão mais recente e, se tiver, vai baixar as diferenças para o seu computador.

15. Git rebase: integrando todas as alterações de um branch em outra branch
O git rebase move e combina sequências de commits para uma nova branch de uma forma mais linear. Uma das diferenças do rebase para o merge é que o rebase mantém esse histórico do projeto de uma forma mais linear e organizada. O comando é simples, mas todo o conceito de como ele funciona é mais complexo. Para rodar, basta usar git rebase <branch>.

16. Git stash: criando um backup das alterações atuais do seu projeto
O git stash serve para guardar ou arquivar as alterações feitas por um determinado tempo. Ele é bem útil quando precisa-se mudar de contexto rápido e ainda não está pronto para fazer um commit, ou também quando precisa-se fazer um teste de uma nova linha de pensamento e não quer perder tudo que já fez antes de ter certeza que a nova abordagem funcionará. Para usar o comando git stash e para recuperar as alterações, basta usar git stash pop.

17. Git clone: baixando o código fonte de um repositório!
Consegue-se clonar, ou copiar, o projeto para o computador. Pode-se clonar um repositório localmente, fazendo uma cópia dele. Para isso, basta rodar git clone /caminho/para/o/repositório. Ou também pode clonar um repositório remoto e para isso usar git clone “url”.

#Bibliografia
https://blog.betrybe.com/git/#1 - visto em 12/04/2022


