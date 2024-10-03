App de receitas real que possibilita o cliente a fazer o login autenticado via token para gerenciar suas receitas com imagens, tags, ingredientes e muito mais. Não contém front-end (porém um dia posso fazer), é focado em desenvolver, documentar, manter RESTful APIs, escaláveis e seguras, construída usando Django e PostgreSQL. O projeto utiliza Docker para facilitar a conteinerização e implantação, e o Django REST Framework (DRF) para criar uma API RESTful robusta para o gerenciamento de receitas.

Funcionalidades:

	•	Operações CRUD: Criar, ler, atualizar e deletar receitas.
 	•	Filtro e Pesquisa: Pesquisar receitas conforme tags, ingredientes, quantidade de ingredientes, etc.
	•	Categorização de Receitas: Imagens para suas receitas, tags para filtrar, adicionar quantos ingredientes quiser, o tempo, o preço, a descrição, etc.
	•	Autenticação: Autenticação segura de usuários usando o sistema integrado do Django via Token.
	•	Banco de Dados PostgreSQL: Armazenamento e gerenciamento eficiente de dados relacionais.
	•	Docker: Ambiente conteinerizado para fácil configuração e implantação.

Stack Tecnológico:

	•	Django: Framework backend para Python.
	•	Django REST Framework: Framework REST API para Django.
	•	PostgreSQL: Sistema de gerenciamento de banco de dados relacional.
	•	Docker: Conteinerização para desenvolvimento e produção.
 	•	Github Actions: manuntenção de pipelines, CI/CD em produção
  	•	SwaggerUI: Documentação completa das RESTful APIs, contendo: endpoints, testes autenticados, requisições, schemas e etc. Consulte em localhost/api/docs.

Instalação:

	1.	Clone este repositório.
	2.	Configure a sua imagem do Docker (ligue ele localmente).
	3.	Suba seu servidor com: docker-compose up (ele ja vai instalar tudo pois foi configurado no Dockerfile, fique tranquilo)
 	4.	Consulte e teste a documentação das APIs em: http://127.0.0.1:8000/api/docs/
  	5.      Não se esqueça de autenticar seu user: em apis user, /api/user/token/ , faça login, copie e cole o token gerado, e em cima da page, clique em "Authorize", clique em tokenAuth, e digite no campo, desse jeito: Token: xxxxxxxxxxxxxxxxxxxxx 
