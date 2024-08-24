# avaliacao-jp
avaliacao-jp Sávio Souza Lopes

***Códigos que Possuímos:***

------------------------------------------------------------------

- git init;
- git status;
- git add <filename ou . >;
- git rm --cached <file> / git restore --staged <filename ou . >;
- git branch;
- git checkout <branchname>;
- git checkout -b <branchname>;
- git commit -m "<description>";
- git push;
- git branch -D <branchname>;
- git fetch;
- git pull;

------------------------------------------------------------------

- Git init;
Inicializa um novo repositório Git em um diretório existente.
Cria um subdiretório .git que contém todos os arquivos
necessários para o repositório.
Para desfazer a inicialização, exclua o diretório .git.

---

- Git status;
Exibe o estado atual do repositório.
Mostra arquivos modificados, novos arquivos e arquivos
preparados para commit.
Não há necessidade de reverter, pois apenas exibe informações.

---

- Git add <filename ou . >;
Adiciona arquivos ao índice (staging area).
Prepara os arquivos especificados para o próximo commit.
Use git rm --cached <file> para remover os arquivos da staging
area.

---

- Git rm --cached <file>;
Remove arquivos do índice (staging area).
Os arquivos são removidos da staging area, mas não do diretório
de trabalho.
Adicione novamente os arquivos com git add <filename ou . >.

---

- Git branch;
Lista todas as branchs locais existentes
git branch -r Lista todas as branchs remotas
git branch -a Lista todas as branchs remotas e locais

---

- Git checkout <branchname>;
Muda para a branch especificada.
O diretório de trabalho é atualizado para refletir o estado da
branch.
Para voltar à branch anterior, use git checkout <previousbranchname>.

---

- Git checkout -b <branchname>;
Cria uma nova branch e muda para ela.
Uma nova branch é criada e você é movido para essa nova branch.
Use git branch -D <branchname> para excluir a branch e git
checkout <previous-branchname> para voltar à branch anterior.

---

- Git commit -m "<description>";
Faz um commit das mudanças no índice com uma mensagem
descritiva.
As mudanças na staging area são salvas no repositório com a
mensagem fornecida.
Use git reset --soft HEAD~1 para desfazer o último commit
mantendo as mudanças no índice, ou git reset --hard HEAD~1 para
desfazer o commit e as mudanças.

---

- Git merge <branch>;
Realiza o merge da branch ATUAL na Branch informada

---

- Git push;
Envia commits do repositório local para o repositório remoto.
Os commits locais são enviados para a branch correspondente no
repositório remoto.
Use git revert <commit-hash> para criar um novo commit que
desfaz as mudanças do commit específico.

---

- Git branch -D <branchname>;
Exclui a branch especificada.
A branch é removida do repositório local.
Não há como reverter diretamente. Se necessário, crie a branch
novamente a partir de um commit específico.

---

- Git fetch;
Baixa objetos e referências do repositório remoto.
Atualiza o repositório local com informações do repositório
remoto sem mesclar.
Não há necessidade de reverter, pois apenas atualiza as
referências locais.

---

- Git pull;
Baixa objetos e referências do repositório remoto e mescla com a
branch atual.
Mescla as mudanças do repositório remoto na branch local.
Use git reset --hard <commit-hash> para reverter o estado da
branch local ao commit anterior ao pull.

------------------------------------------------------------------

Comandos  **GitHub – SSH** 

*Clonar SSH Passo a Passo*

- SSH - GitBash
Verificar se existe chave ssh.
ls -al ~/.ssh

- Adicionar uma nova chave. (ID)
ssh-keygen -t ed25519 -C "your_email@example.com"

- Inicializar agente-ssh.
eval "$(ssh-agent -s)"

- Adicionar chave ssh ao agente.
ssh-add ~/.ssh/id_ed25519

- Copiar chave ssh.
clip < ~/.ssh/id_ed25519.pub

- Adicionar chave no github
Github -> Settings -> SSH and GPG keys -> New SSH key -> Colar
*Coloque um título que identifique a chave*
Ex: SENAC-SALA-206-PCXPTO

- Testar conexão
ssh -T git@github.com
yes


<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portfólio 🐢</title>
    <link rel="stylesheet" href="./styles/index.css">
</head>
<body>
    <div class="container">
         <h1>Escolha uma Opção</h1>
         <a href="./html-basico.css">Inicio</a>
    </div>
</body>
</html>



!DOCTYPE html> 

 

<html lang="pt-br"> 

<head> 

    <meta charset="UTF-8"> 

    <meta name="author" content="Sávio Lopes"> 

    <meta name="keywords" content="portfolio, curriculo, Sávio"> 

    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 

    <title>Portfolio</title> 

    <link rel="stylesheet" href="styles/1-html-básico.css"> 

</head> 

<body> 

    <header> 

  <h1>Página HTML</h1> 

  <a class= "btn" href="index.html">Voltar</a> 

</header> 

 

     

  <main> 

 

  </main class="container"> 

  <section> 

    <h2>Seção de listas</h2> 

    </section> 

    <div> 

        <h3> 

            lista não ordenada  

            <ul> 

                <li> 

                    item 1</li> 

                <li>item 2</li><li>item 3</li> 

            </ul> 

        </h3> 

    </div> 

    <div> 

        <h3>lista ordenada </h3> 

        <ol> 

            <li> 

                item 1</li> 

            <li>item 2</li><li>item 3</li> 

        </ol> 

 

    </div> 

 

    <section> 

        <h2>Seção de Imagem e vídeo</h2> 

        </section> 

        <img src="./giphy.gif" alt=""> 

        <div></div> 

        <idframe><iframe width="560" height="315" src="https://youtu.be/bpZvg_FjL3Q?si=AHUT-EJnF2SNofNE" title="Vídeo Youtube" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></idframe> 

        <section class ="last"> 

            <h2>Seção de Formulário</h2> 

            </section> 

            <form> 

                <label for="nome"> Nome:</label> 

                <input type="text" id="nome" name="nome" placeholder="Seu nome" required> 

                <div> 

                

 

                <label for="email">Email: </label> 

                <label><input type="email" name="email" id="email" placeholder="bananinha@gmail.com" required> 

<div></div> 

                    <label for="senha">Senha: </label> 

                <label><input type="password" name="senha" id="senha" placeholder="12345678"required> 

                    <div></div> 

                <button type="submit">Salvar</button> 

                <button type="reset">Limpar</button> 

 

            </form> 

   

   

            <footer> 

<p> 

    &copy; 2024 - direitos reservados a Sávio Lopes 

</p> 

 

 

  </footer> 

</body> 

</html> 