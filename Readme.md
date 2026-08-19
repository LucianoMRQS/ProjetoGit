Criando o repositório local:

    git init                                    Inicializa o repositório local.
    git branch -M "main"                        Altera o nome da brach.
    git remote add origin <github_url>          Conecta o repositório local ao github.
    git push -u origin main                     Sincroniza o repositório do github com o repositório local.

Pós repositório criado:

    git add <file_name ou .>                    Prepara a branch com um arquivo específico (file_name) ou todos (.).
    git restore --staged <file_name ou .>       Remove da branch, um arquivo específico (file_name) ou todos (.)
    git commit -m "Rótulo de versionamento"     Cria o commit da branch e o rótulo da versão.
    git push origin main                        Envia os dados para o repositório do Github.
    git status                                  Retorna o resumo do status após cada comando.