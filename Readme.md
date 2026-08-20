Criando o repositório:

    git init                                Inicializa o repositório local.
    git branch -M "main"                    Altera o nome da branch principal para main.
    git remote add origin <github_url>      Conecta o repositório local ao GitHub.
    git push -u origin main                 Sincroniza os repositórios web e local, e define o rastreamento padrão.
    clear                                   Limpa a tela do terminal.

Manipulando o repositório:

    git add <file_name ou .>                Prepara arquivos específicos ou todos para o commit (Staging Area).
    git restore --staged <file_name ou .>   Remove arquivos da Staging Area mantendo as alterações no código.
    git commit -m "Mensagem"                Salva o estado dos arquivos em staging com um rótulo no histórico.
    git commit --amend -m "Nova mensagem"   Altera a mensagem ou conteúdo do último commit (se não executado push).
    git push origin main                    Envia os dados da branch local para o repositório remoto.
    git status                              Exibe o estado atual do repositório.

Ramificando e Navegando:

    git checkout -b "nova-branch"           Cria e alterna imediatamente para uma nova branch.
    git checkout main                       Alterna para a branch principal (main).

Integrando alterações:

    git merge criando-ramificacao           Une o histórico da branch informada dentro da branch atual.
                                                i : insert
                                                ESC : termina o insert
                                                :x : salva
                                                ENTER

Auditando o repositório:

    git log                                 Exibe o histórico detalhado de commits com rolagem.
                                                Teclas up/down ou j/k : rolagem dos logs.
                                                q : sair do log
    git log -1 --oneline                    Exibe apenas o último commit em formato resumido de uma linha.

Comandos Por Estudar

    Obtendo e Atualizando Código (Essencial em Equipe):
    
        git clone <github_url>              Clona um repositório web para a sua máquina local.
        git pull origin <branch>            Baixa e aplica automaticamente no seu código as alterações do servidor remoto.
        git fetch                           Baixa o histórico remoto sem alterar seu o local, permitindo ver mudanças antes de unificar.
    
    Navegação Moderna de Branches:
    
        git branch — Lista todas as branches locais do repositório.
        git switch <nome-da-branch> — Alterna para uma branch existente (comando moderno equivalente ao checkout).
        git switch -c <nova-branch> — Cria e alterna para a nova branch (substituto moderno de checkout -b).
        git branch -d <nome-da-branch> — Deleta com segurança uma branch local que já foi unificada via merge.
    
    Guardando Alterações Temporariamente (Stash):
    
        git stash — Oculta e guarda suas alterações não salvas na gaveta, deixando a workspace limpa.
        git stash pop — Recupera a última alteração salva na gaveta e aplica de volta no seu código.
        git stash list — Lista tudo o que você tem guardado na gaveta temporária.
    
    Inspecionando e Desfazendo Erros:
    
        git diff — Mostra linha por linha o que foi alterado antes de você rodar o git add.
        git restore <file_name> — Descarta alterações locais de um arquivo, voltando ao estado do último commit.
        git reset --soft HEAD~1 — Desfaz o último commit mantendo as alterações salvas na Staging Area.
        git reset --hard HEAD~1 — Desfaz o último commit e apaga permanentemente todas as alterações daquele commit.
    
    Reorganizando Histórico:
    
        git rebase main — Aplica seus commits do topo da branch main, mantendo o histórico de commits linear e limpo.