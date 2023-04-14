# Alura Space - CRUD de Fotografias de Galáxias com Django

Este é um projeto desenvolvido dem Python e Django, que consiste em um CRUD (Create, Read, Update, Delete) para fotografias de galáxias. As imagens são persistidas na Amazon S3.

## Tecnologias utilizadas

- Python
- Django
- HTML5
- CSS3
- Amazon S3

## Executando o projeto

Para executar o projeto localmente, é necessário ter o Python e o Django instalados em seu computador, bem como uma conta na Amazon Web Services com acesso ao serviço S3.

1. Clone o repositório:

```
git clone https://github.com/dara-ingrid/alura-space.git
```

1. Acesse o diretório do projeto:

```
cd alura-space
```

1. Crie um ambiente virtual e instale as dependências:

```
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

1. Configure as variáveis de ambiente para acesso à S3:

```
export AWS_ACCESS_KEY_ID=<sua_access_key_id>
export AWS_SECRET_ACCESS_KEY=<sua_secret_access_key>
export AWS_STORAGE_BUCKET_NAME=<seu_bucket_name>
```

1. Execute as migrações do banco de dados:

```
python manage.py migrate
```

1. Inicie o servidor:

```
python manage.py runserver
```

1. Acesse o site em seu navegador:

```
http://localhost:8000
```

## Como utilizar o CRUD

O CRUD é composto por quatro operações básicas:

- Criação de uma nova fotografia de galáxia
- Listagem das fotografia de galáxias cadastradas
- Atualização de uma fotografia de galáxia existente
- Exclusão de uma fotografia de galáxia existente

Para acessar as funcionalidades do CRUD, acesse a página principal do site e utilize o menu de navegação.
