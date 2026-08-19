Criando o repositório:

    git init                                    Inicializa o repositório local.
    git branch -M "main"                        Altera o nome da brach.
    git remote add origin <github_url>          Conecta o repositório local ao github.
    git push -u origin main                     Sincroniza o repositório do github com o repositório local.
    clear                                       Limpa a tela.

Manipulando o repositório:

    git add <file_name ou .>                    Prepara a branch com um arquivo específico (file_name) ou todos (.).
    git restore --staged <file_name ou .>       Remove da branch, um arquivo específico (file_name) ou todos (.)
    git commit -m "Rótulo de versionamento"     Cria o commit da branch e o rótulo da versão.
    git push origin main                        Envia os dados para o repositório no Github.
    git status                                  Retorna o resumo do status após cada comando.

Ramificando o repositório

    git checkout -b "criando-ramificacao"       Cria uma nova branch chamada "criando-ramificacao".

Sobrescrevendo o respositório principal

    git checkout main                           Acessa uma branch específica, neste exemplo a main.
    git merge criando-ramificacao               A partir da main, sobrescreve os novos dados na branch principal.
                                                Isso exige que você crie uma mensagem para o merge.
                                                    i : insert
                                                    ESC : termina o insert
                                                    :x : salva
                                                    ENTER