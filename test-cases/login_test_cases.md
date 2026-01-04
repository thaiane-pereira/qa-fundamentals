### CT-01 – Login com credenciais válidas

Pré-condição:
Usuário cadastrado no sistema

Passos:
1. Acessar a página de login
2. Informar usuário válido
3. Informar senha válida
4. Clicar no botão "Entrar"

Resultado esperado:
Usuário deve ser autenticado e redirecionado para a página inicial.

### CT-02 – Tentativa de login com credenciais inválidas
Pré-condição:
Usuário não cadastrado no sistema

Passos:
1. Acessar a página de login
2. Informar usuário inválido
3. Informar senha inválida
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e deve exibir uma mensagem como "Usuário ou senha inválidos". 

### CT-03 – Tentativa de login com username inexistente e senha válida de outro usuário

Pré-condição:
Existe pelo menos um usuário cadastrado no sistema

Passos:

1. Acessar a página de login
2. Informar um username que não pertence a nenhum usuário cadastrado
3. Informar uma senha válida de um usuário existente
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e deve exibir uma mensagem como "Usuário ou senha inválidos". 

### CT-04 – Tentativa de login com senha inválida e usuário válido
Pré-condição:
Usuário cadastrado no sistema

Passos:
1. Acessar a página de login
2. Informar usuário válido
3. Informar senha inválida
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e deve exibir uma mensagem como "Usuário ou senha inválidos".

### CT-05 – Tentativa de login com campos de usuário e senha vazios
Pré-condição:
Nenhuma

Passos:
1. Acessar a página de login
2. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e deve exibir uma mensagem informando que os campos Usuário e Senha são obrigatórios.

### CT-06 – Tentativa de login com campo usuário vazio e senha preenchida

Pré-condição:
Usuário cadastrado no sistema

Passos:
1. Acessar a página de login
2. Deixar o campo Usuário vazio
3. Informar senha válida
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e o sistema deve exibir uma mensagem informando que o campo Usuário é obrigatório.

### CT-07 – Tentativa de login com campo senha vazio e usuário preenchido

Pré-condição:
Usuário cadastrado no sistema

Passos:

1. Acessar a página de login
2. Informar usuário válido
3. Deixar o campo Senha vazio
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e o sistema deve exibir uma mensagem informando que o campo Senha é obrigatório.

### CT-08 – Tentativa de login com espaços em branco nos campos

Pré-condição:
Usuário cadastrado no sistema

Passos:

1. Acessar a página de login
2. Informar Usuário válido com espaço em branco no início/final do campo
3. Informar Senha válida com espaço em branco no início/final do campo
4. Clicar no botão "Entrar"

Resultado esperado:
O sistema deve ignorar os espaços inseridos nos campos e o deve ser realizado.

### CT-09 – Tentativa de login com username com tamanho acima do limite permitido

Pré-condição:
Existe ao menos um usuário cadastrado no sistema

Passos:

1. Acessar a página de login
2. Informar um username com quantidade de caracteres acima do limite permitido
3. Informar qualquer senha
4. Clicar no botão "Entrar"

Resultado esperado:
O login não deve ser realizado e o sistema deve exibir uma mensagem de validação informando que o username excede o limite permitido.

### CT-10 – Tentativa de login após múltiplas tentativas consecutivas inválidas

Pré-condição:
Usuário cadastrado no sistema

Passos:

1. Acessar a página de login
2. Informar usuário válido
3. Informar senha inválida
4. Repetir a tentativa por múltiplas vezes consecutivas
5. Tentar realizar o login novamente

Resultado esperado:
O sistema deve bloquear temporariamente novas tentativas ou exibir uma mensagem de alerta sobre múltiplas tentativas inválidas.
