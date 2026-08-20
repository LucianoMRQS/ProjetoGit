Comandos Em Estudo

    Obtendo e Atualizando Código (Essencial em Equipe):
    

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
