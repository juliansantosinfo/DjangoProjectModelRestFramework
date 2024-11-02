# DjangoProjectModelRestFramework

Este repositório serve como um template para projetos Django REST Framework, podendo ser utilizado como base para novos repositórios no GitHub. Ele oferece uma configuração pré-pronta com diversas bibliotecas úteis para o desenvolvimento de APIs robustas e escaláveis, gerenciadas pelo Poetry.

## Recursos

Este template inclui as seguintes bibliotecas e funcionalidades:

* **Django:** Framework web Python de alto nível para desenvolvimento rápido.
* **Django REST Framework:** Toolkit poderosa e flexível para construir APIs Web.
* **dj-rest-auth:**  Fornece um conjunto de endpoints REST para autenticação e registro de usuários, integrando-se com o django-allauth.
* **django-admin-interface:**  Interface moderna e responsiva para o painel de administração do Django.
* **django-allauth:**  Aplicação Django integrada para autenticação, registro, gerenciamento de contas e autenticação social de terceiros.
* **django-cors-headers:**  Aplicação Django para lidar com as configurações de CORS (Cross-Origin Resource Sharing), permitindo que sua API seja acessada por diferentes domínios.
* **django-environ:**  Permite a configuração de projetos Django usando variáveis de ambiente.
* **django-filter:**  Fornece um sistema genérico para filtrar querysets do Django based nas opções de URL.
* **gunicorn:** Servidor WSGI HTTP para aplicações Python.
* **psycopg2-binary:** Adaptador PostgreSQL para Python.
* **python-dotenv:**  Lê as variáveis de ambiente do arquivo .env.
* **requests:**  Biblioteca HTTP para Python.
* **whitenoise:**  Serve arquivos estáticos para aplicações web Python.

## Como usar este template

1. Clique no botão "Use this template" no GitHub para criar um novo repositório a partir deste template.
2. Clone o novo repositório para sua máquina local.
3. Crie um ambiente virtual e instale as dependências usando o Poetry:

```bash
python -m venv .venv
source .venv/bin/activate
poetry install
```

4. Configure as variáveis de ambiente no arquivo `.env`. Um exemplo de `.env` é fornecido como `.env.example`.
5. Execute as migrações:

```bash
poetry run python manage.py migrate
```

6. Crie um superusuário:

```bash
poetry run python manage.py createsuperuser
```

7. Inicie o servidor de desenvolvimento:

```bash
poetry run python manage.py runserver
```

## Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## Licença

Este projeto é licenciado sob a licença MIT.


## Observações

*  Lembre-se de configurar suas variáveis de ambiente, especialmente as relacionadas à autenticação e ao banco de dados.
* Este README deve ser atualizado com informações específicas do seu projeto após utilizar o template.  Substitua as informações genéricas por detalhes relevantes para o seu projeto.
*  Explore as configurações e funcionalidades oferecidas pelas bibliotecas incluídas para adaptar o projeto às suas necessidades.
* As dependências do projeto são gerenciadas pelo Poetry.  O arquivo `pyproject.toml` contém as informações necessárias. Utilize os comandos do Poetry para gerenciar as dependências (ex: `poetry add <pacote>` para adicionar um novo pacote).
