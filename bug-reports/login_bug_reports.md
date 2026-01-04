### BUG-01 – Mensagem de erro de login exibida diferente do esperado e toast não responsivo

Ambiente:
Web – Chrome 120 – MacOS Sequoia Versão 15.6.1

Caso de teste relacionado:
CT-02, CT-03, CT-04, CT-05

Pré-condição: 
Variável conforme o caso de teste executado

Passos para reproduzir:
1. Acessar a página de login
2. Informar usuário inválido
3. Informar senha inválida
4. Clicar no botão "Entrar"

Resultado esperado:
O sistema não deve realizar o login e deve exibir uma mensagem como "Usuário ou senha inválidos" em um toast responsivo.

Resultado obtido:
O sistema não realiza o login, porém a mensagem exibida é diferente do esperado e o toast de erro não se adapta corretamente ao tamanho da tela.

Severidade:
Média

Status:
Aberto

### BUG-02 – O sistema não realiza o login quando é inserido espaço nos campos
Caso de teste relacionado:
CT-08

Pré-condição:
Usuário está cadastrado no sistema

Passos para reproduzir:
1. Acessar a página de login
2. Informar usuário válido com espaço no final
3. Informar senha válida com espaço no final
4. Clicar no botão "Entrar"

Resultado esperado:
O sistema deve realizar o login normalmente, ignorando os espaços informados pelo usuário.

Resultado obtido:
O sistema não realiza o login e informa que usuário e senha estão incorretos.

Severidade:
Média

Status:
Aberto

### BUG-03 – O sistema não acusa erro ao inserir usuário com grande quantidade de caracteres
Caso de teste relacionado:
CT-09

Passos para reproduzir:
1. Acessar a página de login
2. Informar usuário com quantidade elevada de caracteres (acima de 10)
3. Informar senha válida
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e o sistema deve exibir uma mensagem de validação informando que o username excede o limite permitido.

Resultado obtido:
O sistema somente acusa erro de usuário incorreto e não informa sobre o limite excedido.

Severidade:
Média

Status:
Aberto

### BUG-04 – O sistema não bloqueou o acesso após múltiplas tentativas incorretas
Caso de teste relacionado:
CT-10

Passos para reproduzir:
1. Acessar a página de login
2. Informar usuário válido
3. Informar senha inválida
4. Repetir a tentativa por múltiplas vezes consecutivas
5. Tentar realizar o login novamente

Resultado esperado:
O sistema deve bloquear temporariamente novas tentativas ou exibir uma mensagem de alerta sobre múltiplas tentativas inválidas.

Resultado obtido:
O sistema não bloqueia novas tentativas e nem exibe alerta sobre múltiplas tentativas, continua permitindo o usuário tentar realizar o login novamente

Severidade:
Alta

Status:
Aberto