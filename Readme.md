git add <"file_name" or ".">         Prepara um arquivo específico (file_name) ou todos (.) para o commit.
git commit -m "Comentário"           Cria um rótulo para o commit que será enviado.
git push origin main                 Envia os dados para o repositório do Github.

git status                           Retorna oque esta separado, aguardando o commit.
                                     Caso seja dado após o status, mostrará o seguinte:
                                        Após "add" :
                                            On branch main
                                            Your branch is ahead of 'origin/main' by 1 commit.
                                            (use "git push" to publish your local commits)
                                        Após "commit" : 