# Trabalho-de-Teste-Caixa-Branca-e-Caixa-Preta
Trabalho visa realizar o Teste Caixa Branca e Caixa Preta no projeto https://github.com/cleberleao/oficina-spring-boot, assim como documentar os testes nesse repositório.

Testes de Caixa Branca 


Conhecimento Interno do Código:


Testes unitários focados no UserService
Verificação da lógica de validação de e-mail único


Cobertura Verificada:

Fluxos alternativos (e-mail já existente)
Tratamento de exceções customizadas

--------------------------------------------------
Testes de Caixa Preta


Testes via Swagger UI:


Validação dos endpoints REST
Verificação dos códigos de status HTTP
Análise dos contratos de resposta

Casos de Teste Executados:


Cenário	Entrada	Resultado Esperado

E-mail novo	novo@email.com	HTTP 201 (Created)

E-mail duplicado	existente@email.com	HTTP 403 (Conflict)

Formato inválido	email_invalido	HTTP 401 (Bad Request)

Criação de usuario com token de autentificação no Swagger:
![Criação de usuario](https://github.com/user-attachments/assets/7dd38e65-7c9f-46bf-90d2-d2c651b9fdf1)

Retorno de aprovação de usuario no Swagger:
![Retorno de aprovação](https://github.com/user-attachments/assets/4d4f49a3-45f3-4c5e-86e3-9e8c4ab6621b)

Conclusão
O projeto demonstra uma boa aplicação dos princípios de teste, com:

Caixa Branca com Foco na qualidade interna do código e lógica de negócio.

Caixa Preta com Garantia do comportamento esperado da API.
