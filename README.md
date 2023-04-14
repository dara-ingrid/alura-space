# Aluraspace

Aluraspace é um projeto de um CRUD de fotografias do espaço desenvolvido com Python e Django, onde as imagens são persistidas no AWS S3. Este projeto é resultado do curso "Desenvolvimento Python com Django" da Alura.

## Requisitos

- Python 3.x
- Django 3.x
- Django Storages
- Boto3

## Como executar o projeto

1. Clone o repositório:

```
git clone https://github.com/seu-usuario/aluraspace.git
```

1. Crie um ambiente virtual:

```
python3 -m venv env
```

1. Ative o ambiente virtual:

```
source env/bin/activate
```

1. Instale as dependências:

```
pip install -r requirements.txt
```

1. Crie um arquivo `.env` na raiz do projeto com as variáveis de ambiente necessárias:

```
SECRET_KEY=chave_secreta_do_django
DEBUG=True
AWS_ACCESS_KEY_ID=<sua-access-key-id>
AWS_SECRET_ACCESS_KEY=<sua-secret-access-key>
AWS_STORAGE_BUCKET_NAME=<nome-do-seu-bucket>
AWS_S3_REGION_NAME=<região-do-seu-bucket>
```

Você pode gerar uma nova chave secreta do Django executando o script `secret_key_generator.py`. Para isso, siga os passos abaixo:

1. Execute o script `secret_key_generator.py`:

```
python secret_key_generator.py
```

1. Copie a chave gerada e adicione ao arquivo `.env` como o valor da variável `SECRET_KEY`.
2. Execute as migrações do banco de dados:

```
python manage.py migrate
```

1. Inicie o servidor:

```
python manage.py runserver
```

1. Acesse o projeto em `http://localhost:8000/`

## Como contribuir

1. Faça um fork do projeto
2. Crie uma branch para a sua feature: `git checkout -b minha-feature`
3. Faça suas alterações e adicione os arquivos modificados: `git add .`
4. Faça um commit com as suas alterações: `git commit -m "Minha feature"`
5. Envie suas alterações para o seu repositório no Github: `git push origin minha-feature`
6. Abra um Pull Request no repositório original

<h3 align="center">
Feito com ❤️ por <a href="https://www.linkedin.com/in/dara-ingrid/">Dara Ingrid</a>
</a>
</h3>
