# NLW Expert Python
Tag Generator é uma aplicação web desenvolvida com Flask que permite aos usuários criar e personalizar tags em forma de códigos de barras. Utilizando bibliotecas poderosas como Pillow e python-barcode, esta aplicação oferece uma interface intuitiva para a geração de códigos de barras, suportando diversos formatos.

## Status do Projeto
🚧 Em desenvolvimento 🚧

## Índice
- [Começando](#começando)
- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Uso](#uso)
- [Comandos Úteis](#comandos-úteis)
- [Tecnologias](#tecnologias)
- [Contribuição](#contribuição)

## Começando
- Para rodar esta aplicação localmente, siga os passos abaixo.

## Pré-requisitos
- Python 3.12
- pip
- virtualenv

## Instalação
1. Clone este repositório:
```bash
git clone https://github.com/Edufreitass/nlw-expert-python.git
```

2. Crie e ative um ambiente virtual:
```bash
py -m venv .venv
source .venv/Scripts/activate  # Windows/Git Bash
```

3. Instale as dependências:
```bash
pip install -r requirements.txt
```

## Uso
Para iniciar a aplicação, execute:
```bash
$ py run.py
```

Saída
```bash
 * Serving Flask app 'src.main.server.server'
 * Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:3000
 * Running on http://000.000.0.0:3000
Press CTRL+C to quit
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 000-000-000
```

Acesse a aplicação via navegador em http://localhost:3000

O retorno deverá ser algo como:
```html
<html lang="en">
  <head>
    <title>404 Not Found</title>
  </head>
  <body>
    <p>The requested URL was not found on the server. If you entered the URL manually please check your spelling and try again.</p>
  </body>
</html>
```

## Comandos Úteis
```bash

# Verificar quais arquivos estão na area de stage para serem commitados
$ git status

# Adicionar os arquivos que você deseja commitar
$ git add .

# Mensagem do commit, use boas práticas, siga a convenção do "Conventional Commits", link -> https://www.conventionalcommits.org/pt-br/v1.0.0-beta.4/#resumo
$ git commit -m "feat: Adding Amazing Feature"

# Realizar o push (subida) do seu código para o github
$ git push

# Gera o arquivo de configuração  do pylint.
$ pylint --generate-rcfile > .pylintrc

# Após as configurações do pre-commit serem adicionadas, para executar a instalação delas use:
$ pre-commit install

# Caso você decida contribuir e adicionar uma nova dependência, após fazer o pip install XPTO, execute o pip freeze para adicionar no requirements.txt as dependências que foram instaladas.
$ pip freeze > requirements.txt

# Executa o pytest com cobertura de código
$ pytest --cov=.

# Além de executar o pytest com cobertura de código, ele gerá o relátorio HTML da cobertura mais detalhada.
$ pytest --cov=. --cov-report=html
```

## Tecnologias
- **Python 3.12.1** - Linguagem de Programação
- **Flask** - Framework Web
- **Cerberus, pillow, python-barcode** - Bibliotecas para validação de dados, manipulação de imagens e geração de códigos de barras
- **pre-commit, pylint, pytest, pytest-cov** - Ferramentas para qualidade de código e testes
- **Virtualenv** - Ferramenta para criação de ambientes virtuais

## Contribuição
Contribuições são sempre bem-vindas! Para contribuir, por favor:

1. Faça um fork do projeto.
2. Crie uma nova branch (git checkout -b feature/AmazingFeature).
3. Faça commit das suas mudanças (git commit -m 'feat: Add some AmazingFeature').
4. Faça push para a branch (git push origin feature/AmazingFeature).
5. Abra um Pull Request.
