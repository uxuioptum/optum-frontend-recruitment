# Seja bem-vindo!
Este é o teste de recrutamento da Optum Global Solutions para desenvolvedor React.

# Introdução
O objetivo deste teste é avaliar o seu conhecimento e experiência com React e libs relacionadas a esta tecnologia.
O que será desenvolvido neste exercício é a criação de uma lista de afazeres, mais conhecida como TODO List.
* Para que o usuário consiga utilizar sua lista de afazeres, é preciso estar autenticado.

# A aplicação precisa:
* Ser Single Page Aplication (SPA) e desenvolvida em React;
* Conter 3 rotas:
  * A de login. Usuários logados e não logados tem acesso;
  * A da TODO List. Somente usuários logados tem acesso;
  * A rota que somente usuários logados como administradores tem acesso.
  
# Rotas
**LOGIN:**
* Deve conter um formulário para que o usuário se autentique com um email e senha;
  * Utilize a imaginação! Esta autenticação pode ser um mock, para evitar consumir uma API rest.
  * Dica: Você pode criar um [token JWT](https://jwt.io) para simular a autenticação. No "payload" do token você pode inserir os dados do usuário para a autenticação.
* A página de login não deve ser acessível quando o usuário já estiver autenticado.

**TODO List:**
* Deve exibir a lista de afazeres para que o usuário possa:
  * Visualizar as tarefas que estão ou não completas;
  * Cadastrar uma nova tarefa;
  * Editar uma tarefa existente;
  * Excluir uma tarefa existente.
* Somente usuários autenticados podem ter acesso a TODO List.

**ADMIN:**
* Esta rota precisa conter somente um título informando que é a página de administradores;
* Somente usuários autenticados, com papel de "admin", podem ter acesso a esta rota.

# Acesso a API
* Para a busca da lista de afazeres, pode ser utilizado o endpoint: https://jsonplaceholder.typicode.com/todos
  * A API "jsonplaceholder" somente simula requisições para inserção, edição e exclusão. Portanto, você pode
usar um mock para inserir, editar ou excluir o dado desejado ao chamar os respectivos serviços.
* Caso precise filtrar algum dado, leia a seção "Routes": [Json Server #Routes](https://github.com/typicode/json-server#routes)

# Regras
* Ao autenticar-se, você é o usuário com id igual a 3;
* Utilize Redux em sua aplicação;
* Crie validações nos formulários e mostre os erros gerados;
* O seu código precisa estar em um repositório público no GitHub;
* Faça um fork do nosso repositório, crie uma branch com seu nome e faça um pull request até a data limite, enviando a sua solução.
* Caso crie o app com "create-react-app", por favor, crie um commit separado por causa dos arquivos que são gerados pelo CRA;
* Você deve publicar a sua aplicação no [Heroku](https://www.heroku.com/);
* Pontos a mais serão contados caso testes automatizados sejam realizados.

# Prazo
O desafio precisa ser realizado em **uma semana** a partir do dia em que o teste foi encaminhado a você.
