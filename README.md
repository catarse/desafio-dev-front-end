# Desafio Pessoa Desenvolvedora Front-end

O desafio consiste na implementação de um projeto utilizando o framework front-end de sua preferência.

O projeto é o Catarsinho, um Catarse com um escopo bem reduzido, onde será possível visualizar os projetos da plataforma, visitar a página do projeto e adicionar um apoio numa "cesta de apoio". Para auxiliar e focar apenas no que importa para nós, estamos fornecendo um layout já pronto (feito utilizando https://bulma.io) e também um conjunto de dados para simular uma API em ambiente local.

Utilizando a API e o layout fornecidos, queremos que você implemente do front-end da aplicação. Esse teste serve para gente entender como você organiza o projeto, componetiza a aplicação, faz a comunicação entre componentes, testa o código, resolve problemas e organiza os commits.

## Requisitos:

- Utilizar o framework de sua preferência (Vue.js, Angular, Svelte, React e etc)
- Criar página de visualização de projetos
  - Mostrar: nome, imagem, progresso da campanha, % arrecadadado e valor arrecadado
- Criar página de detalhes do projeto
  - Mostrar nome, imagem, progresso da campanha, % arrecadadado, valor arrecadado e descrição do projeto
- Na página de detalhes do projeto, mostrar as opções de apoio do projeto e um botão "Apoiar"
  - São 4 opções: R$ 10, R$ 25, R$ 50 e R$ 100.
- Ao clicar em "Apoiar", Os valores na barra de navegação (quantidade de itens e valor total dos apoios) deverão ser atualizados
- O carrinho de apoio (as informações presentes na barra de navegação superior no canto direito) deve manter os itens mesmo mudando de página.

### Bônus
- Implementar os testes unitários de 1 componente (pode ser o que você achar mais importante)
- Implementar algum teste de e2e, por exemplo: navegar na listagem de projetos, clicar num projeto e verificar se a página está com as informações corretas.

Se você conseguir estruturar bem seus commits, facilitando o entendimento de como foi o progresso de cada funcionalidade, além de mostrar como você se organiza, facilitará bastante nossa análise.

Não é necessário implementar todos os pontos, pode enviar com os pontos que conseguir implementar pois analisaremos com o mesmo carinho.

## Configurando API no ambiente local:

Instale o json-server no seu ambiente: https://github.com/typicode/json-server

Depois execute `json-server --watch db.json`. Esse `db.json` é o arquivo que está presente no repositório. São os dados dos projetos.

Acesse `http//localhost:3000/projects` para acessar a listagem de projetos. E `http//localhost:3000/projects/:id` para acessar um projeto apenas.

## Layout
A página home, que lista os projetos (é o arquivo layout-home.html):
![layout-home.html](https://user-images.githubusercontent.com/3025661/134577514-b59b6f91-135d-445d-8620-82304019e9b3.png)

A página de detalhes do projeto (é o arquivo layout-project.html):
![layout-project.html](https://user-images.githubusercontent.com/3025661/134577615-4db721a2-ea01-415a-acb9-7b5d63bc31a0.png)

