# inventory management software

Um sistema simples de gerenciamento de inventário construído com Django.
Os usuários podem adicionar itens de estoque e gerar contas. Todos os dados são armazenados no banco de dados e são renderizados em tempo real

Para executar o projeto, execute os seguintes comandos no diretório do projeto para criar o banco de dados. Ao executar o software pela primeira vez, é necessário executar cada comando para cada app do projeto:

```bash
python manage.py makemigrations homepage
python manage.py migrate homepage
python manage.py makemigrations inventory
python manage.py migrate inventory
python manage.py makemigrations transactions
python manage.py migrate transactions
```

Após a primeira vez, o seguinte pode ser executado para migrar as alterações do modelo em qualquer aplicativo:

```bash
python manage.py makemigrations
python manage.py migrate
```

Use o seguinte comando para executar o servidor:

```bash
python manage.py runserver
```

Use o seguinte comando para criar um usuário administrador:

```bash
python manage.py createsuperuser
```
