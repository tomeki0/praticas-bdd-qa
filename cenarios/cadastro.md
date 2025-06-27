História de usuário: Cadastro de Novo Usuário

Como um novo usuário, 
Quero poder criar uma conta no sistema, 
Para ter acesso às funcionalidades exclusivas.

Cenário 1: Cadastro com credenciais válidas 

Dado que esteja na tela de cadastro
Quando preencher todos os campos com credenciais válidas
E clicar no botão de cadastrar
Então o sistema deve criar a conta do usuário e o redirecionar para a página inicial da aplicação

Cenário 2: Cadastro com e-mail já existente no sistema

Dado que esteja na tela de cadastro
Quando preencher o campo de e-mail com um e-mail já cadastrado no sistema
E preencher todos os outros campos com credenciais válidas
E clicar no botão de cadastrar
Então o sistema deve mostrar uma mensagem de erro informando que aquele e-mail já está cadastrado no sistema
E o sistema deve permanecer na tela de cadastro

Cenário 3: Cadastro com senha que não atende aos requisitos

Dado que esteja na tela de cadastro
Quando preencher o campo de senha com uma senha que não atende aos requisitos
E preencher os demais campos com credenciais válidas
E clicar no botão de cadastrar
Então o sistema deve mostrar uma mensagem de erro informando que a senha não atende os requisitos
E o sistema deve permanecer na tela de cadastro


Cenário 4: Cadastro com campos obrigatórios vazios

Dado que esteja na tela de cadastro
Quando deixar um campo obrigatório vazio
E preencher os demais campos com credenciais válidas
E clicar no botão de cadastrar
Então o sistema não deve criar a conta
E deve mostrar uma mensagem de erro informando que um campo obrigatório está vazio
E deve permanecer na tela de cadastro
