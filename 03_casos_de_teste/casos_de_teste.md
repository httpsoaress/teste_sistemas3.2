Casos de Teste
 --

CT01 – Cadastro de Usuário com Dados Válidos

Requisito: RF13

Descrição: Verificar se o sistema permite o cadastro de usuário com dados válidos.

Pré-condição: Usuário não possui conta cadastrada.

Entrada:

• E-mail válido e não cadastrado

• Senha válida (mínimo 8 caracteres, com maiúscula, minúscula e número)
Resultado Esperado:

• Conta criada com sucesso


• Mensagem de confirmação exibida

• Usuário pode realizar login

--------------------------------------------------------------------------------------------
CT02 – Cadastro com E-mail Duplicado
Requisito: RN01

Descrição: Verificar se o sistema impede cadastro com e-mail já existente.

Pré-condição: Já existe uma conta com o e-mail informado.

Entrada:

• E-mail já cadastrado

• Senha válida

Resultado Esperado:

• Sistema bloqueia o cadastro

• Mensagem informando que o e-mail já está em uso

-------
CT03 – Login com Credenciais Válidas

Requisito: RF14

Descrição: Verificar se o sistema permite login com credenciais corretas.

Pré-condição: Usuário previamente cadastrado.

Entrada:

• E-mail válido

• Senha correta

Resultado Esperado:

• Login realizado com sucesso

• Redirecionamento para página principal

-------
CT04 – Cadastro de Bairro por ADMIN

Requisito: RF01

Descrição: Verificar se um administrador pode cadastrar um novo bairro.

Pré-condição: Usuário autenticado com perfil ADMIN.

Entrada:

• Nome do bairro valido (O nome não pode ser repetido)

• Coordenadas válidas (latitude e longitude)

• Informações obrigatórias preenchidas

Resultado Esperado:

• Bairro cadastrado com sucesso

• Ping exibido corretamente no mapa

------
CT05 – Exclusão de Bairro por ADMIN MASTER

Requisito: RF04 / RN08

Descrição: Verificar se apenas ADMIN MASTER pode excluir bairros.

Pré-condição: Bairro previamente cadastrado.

Entrada:

• Solicitação de exclusão realizada por ADMIN MASTER

Resultado Esperado:

• Bairro removido do sistema

• Avaliações e comentários associados também removidos

-----
CT06 – Edição de Bairro por ADMIN 

Requisito: RF02 / RN08

Descrição: Verificar se apenas ADMIN ou ADMIN MASTER pode editar bairros.

Pré-condição: Bairro previamente cadastrado.

Entrada:

• Solicitação de edição realizada por ADMIN ou ADMIN MASTER

• Seleção de dados a serem alterados (Ex: Nome do bairro)

• Confirmar edição do bairro

Resultado Esperado:

• Bairro Editado

-----
CT07 – Avaliação de Bairro

Requisito: RF05 / RN09

Descrição: Verificar se o usuário consegue avaliar um bairro.

Pré-condição: Usuário autenticado.

Entrada:

• Nota para critério (ex: Segurança = 4)

Resultado Esperado:

• Avaliação registrada com sucesso

• Média do bairro atualizada automaticamente

------

CT08 – Comentário com Conteúdo Permitido

Requisito: RF08

Descrição: Verificar se o usuário consegue publicar comentário válido.

Pré-condição: Usuário autenticado.

Entrada:

• Comentário com até 800 caracteres

• Sem links ou conteúdo proibido

Resultado Esperado:

• Comentário publicado

• Exibição do selo (morador ou visitante)

-----
CT09 – Comentário com Conteúdo Proibido

Requisito: RN11 / RN13

Descrição: Verificar se o sistema encaminha comentário inadequado para moderação.

Pré-condição: Usuário autenticado.

Entrada:

• Comentário contendo link externo

Resultado Esperado:

• Comentário não publicado imediatamente

• Status definido como "pendente"

• Disponível para análise do administrador

-----
CT10 – Filtro por Nome do Bairro

Requisito: Funcionalidade de filtro

Descrição: Verificar se o sistema permite filtrar bairro pelo nome.

Pré-condição: Existem bairros cadastrados.

Entrada:

• Nome parcial ou completo do bairro

Resultado Esperado:

• Sistema retorna apenas bairros correspondentes

----
CT11 – Curtir Comentário

Requisito: RF10

Descrição: Verificar se o usuário pode curtir comentário.

Pré-condição: Comentário previamente publicado.

Entrada:

• Clique no botão “Curtir”

Resultado Esperado:

• Contador de curtidas incrementado

• Sistema impede múltiplas curtidas pelo mesmo usuário

-----
CT12 – Gerenciar usuário

Requisito: RF15

Descrição: Verificar se apenas o ADMIN ou ADMIN MASTER pode excluir ou bloquear perfis de usuário


Pré-condição: Usuario previamente cadastrado.

Entrada:

• ADMIN ou ADMIN MASTER logado

• Selecionar um usuario

• Selecionar opção de exclusão/bloqueio

• Confirmar de exclusão/bloqueio


Resultado Esperado:

• Contador de curtidas incrementado

• Sistema impede múltiplas curtidas pelo mesmo usuário

---
CT13 – Cadastrar endereço

Requisito: RF16

Descrição: Verificar se o usuário pode cadastrar o endereço.


Pré-condição: Usuário não possui conta cadastrada.

Entrada:

• Informar CEP

Resultado Esperado:

• Acessar a tela de cadastro.

• Preencher todos os campos obrigatórios (dados pessoais + endereço).

• Confirmar criação da conta.






