### Instruções para a Avaliação Final

1. **Crie um repositório no GitHub:**
   - Nomeie o repositório como `AvaliacaoFinalJp`.
   - Clone o repositório para sua máquina.
   - Inicialize um **projeto novo** no repositório.

2. **Instale as dependências necessárias:**
   - Instale todas as dependências que utilizamos ao longo do curso.
   - Configure corretamente a estrutura de pastas do projeto.

3. **Banco de Dados:**
   - Crie um banco de dados chamado `Locadora`.
   - No banco, crie as seguintes tabelas com suas respectivas colunas:
     - **Clientes**: `id`, `nome`, `email`, `senha`.
     - **Filmes**: `id`, `titulo`, `classificacaoIndicativa`, `diretor`.
     - **Filmes_Locados**: `id`, `idFilme`, `idCliente`, `dataLocacao`, `dataDevolucao`.

4. **Funcionalidades do Sistema:**
   - **CRUD para Clientes e Filmes:** 
     Implemente todas as operações de criação, leitura, atualização e exclusão para as tabelas **Clientes** e **Filmes**.
   - **Autenticação:**
     - Crie uma rotina de login para validar o acesso dos clientes.
     - Retorne um **token JWT** após o login.
   - **Middleware de Autenticação:**
     - Implemente um middleware para validar o **token JWT** em rotas protegidas.
   - **Rotas Específicas:**
     - Crie duas rotas adicionais:
       - `/filmes/locar`: Permite registrar a locação de um filme por um cliente.
       - `/filmes/devolver`: Permite registrar a devolução de um filme.

5. **Validações:**
   - Certifique-se de validar todas as entradas, como dados do cliente, filmes e tokens.
   - Garanta que as operações sejam consistentes com as regras de negócio (por exemplo, um cliente não pode locar um filme inexistente).