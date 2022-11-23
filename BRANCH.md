# Branch
 São ramificaçoes do projeto, o qual permite varios desenvolvedores trabalharem em diferentes funcionalidades, sem bugar a versão estável.

 Branch main -> que é a branch principal , ou seja, a branch estável da aplicação. versão que é disponibilizada aos clientes.

 Branch developer -> é branch utilizada pelos testers, os quais vão testar as novas funcionalidades, correções de bugs, etc.

 ## outras branchs

 Para cada nova funcionalidade ou correção de bugs é criada uma nova branch

 ### Padrões para criar nomes de branch

!IMPORTANTE! Nomes de branchs não tem acentos nem Ç


 Para correçao de bugs: fix_identificação_do_bug
 Exemplo: fix_botao_delogin, fix_cor_do_cabeçalho


Para novas funcionalidades:
feat_identificação_da_novo_funcionalidade

atualizar documentação: doc_identificação
_da_alteração

Exemplo: doc_adicionada_nova_imagem

Para criação/alteração de tarefas que não interfere no código:
chore_identificação_da_modificacao
Exemplo: chore_atualizando_a_versao_do_banco

## Criação de novas branchs

git checkout -b nome_da_nova_branch

Exemplo:git checkout -b fix_botao_da_tela_login

Obs: o idela é sempre criar branchs a partir da main.

### Listar as branchs existentes
git branch list

### Trocar de branch
git switch nome_da_branch_que_deseja_entregar

Exemplo01: git switch fix_botao_da_tela_login

Exemplo02: git switch main

### Excluir uma branch
git branch -b nome_da_branch_que_deseja_excluir

Exemplo: git branch -b fix_botao_da_tela_de_login

## alterar o nome de uma branch
Primeiramente, certifique-se que esta dentro da branch main, se nao estiver use:
git switch main

Segundo, verifique se a branch main esta atualizada com o comando
git pull origin main

trazer os dados da branch para a  main
git merge nome_da_branch