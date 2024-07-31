# Aprofundando no git e github

## 1. Analisando mudanças:
1. `git log --oneline`:
Esta linha de código mostra em uma linha, todos os commits feitos, com sua hash(id) e o que escreveram no commit;

2. `git log -p`:
Esta linha de código mostra o que foi mudado de um commit para o outro;

3. `git log --graph`:
Esta linha de código mostra uma linha do tempo dos commits mostrando as branches e merges;

4. `git log --pretty ou --format`:
Esta linha de código permite exibir oque voce quiser sobre o comitt;

5. `git show {hash do commit}`:
Basicamente a mesma coisa que o git log -p, porém serve apenas para um commit;

6. `git diff`:
Ele mostra as diferenças entre o ultimo commit e o arquivo atual;

7. `git diff {hash de um commit}..{hash de outro commit}`:
Ele mostras as diferenças de um commit para o outro;

## 2. Organizando projeto:
1. `git branch`:
Mostra a quantidade de branchs no projeto

2. `git branch {nome da ramificacao}`:
Cria uma nova branch;

3. `git switch {nome da ramificação}`:
Agora você está na branch que digitou acima o nome;

4. `git merge {nome da ramificação}`:
Este código preserva o historico antigo inteiro da outra ramificação, e apenas adiciona o que tinha de novo;

4. `git rebase {nome da ramificação}`:
Este código, diferente do `merge`, ele simplesmente vai para a mesma "linha" que a ramificação que vc escolheu, "apagando" a ramificação antiga;

## 3. Manipulando as versões:
1. `git stash`:
Ele vai "engavetar" o código que alterei para poder mexer depois;

2. `git stash pop`:
Ele vai implementar o código que estava "engavetado" ao código novamente;
 
3. `git stash clear`:
Ele vai limpar a lista de stashs;
  
4. `git stash push -m "{mesagem}"`:
É para deixar a stash que você vai engavetar mais descritiva;

5. `git stash apply {indice do stash}`:
Escolhe qual vai ser aplicado dentro do código novamente com base no indice;

6. `git restore`:
Ele vai resetar o código para como o código esta no ultimo commit do github;

7. `git restore --source={hash do commit}`:
Ele vai resetar o código para como estava no commit que digitei;

## 4. Gerando entregas:
1. `git tag v{numero versao}`:
Ele marca uma tag no commit HEAD(ultimo commit);

2. `git tag v{numero versao} {hash do commit}`:
Ele marca uma tag no commit que você colocou acima;

3. `git tag -d {nome da tag}`:
Remove a tag;

4. `git tag -a {nome versao} -m {mensagem}`:
Cria uma tag que tem informações; 

5. `git cherry-pick {hash do commit}`:
Esta função pega traz um commit de uma branch diferente da que voce está, para a branch que vc esta agora;

6. `git blame {arquivo}`:
Mostra quem escreveu a linha de código