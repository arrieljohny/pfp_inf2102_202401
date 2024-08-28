# Projeto: Análise de Sentimentos e Gestão de Tarefas com Jira

## Descrição

Este projeto é um software desenvolvido em Python e organizado na plataforma Jupyter Notebook com o objetivo de coletar informações de tarefas do software de apoio à gestão de projetos Jira. O sistema extrai dados sobre responsáveis, tempo estimado e tempo gasto em cada tarefa. Além disso, analisa os textos descritos nas descrições e comentários das tarefas para classificar os sentimentos presentes no conteúdo textual.

## Funcionalidades

### Coleta de Dados

- **Conexão com a API do Jira**: O sistema se conecta à API do Jira para coletar informações sobre tarefas.
- **Extração de Dados**: Coleta de dados como responsáveis, tempo estimado e tempo gasto em cada tarefa.

### Análise de Sentimentos

- **Análise de Textos**: O sistema realiza uma análise dos textos presentes nas descrições e comentários das tarefas.
- **Classificação de Sentimentos**: Utilização da biblioteca `text2emotion` para classificar os sentimentos expressos nos textos em cinco categorias: Happy, Angry, Surprise, Sad, e Fear.

## Requisitos

- Python 3.8+
- Jupyter Notebook
- Biblioteca `text2emotion`
- Biblioteca `requests` (para conexão com a API do Jira)

## Instalação

1. Clone este repositório:

   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
Para instalar e usar o projeto, siga os seguintes passos:

1. Clone este repositório usando o comando
     `git clone https://github.com/seu-usuario/seu-repositorio.git`.
2. Navegue até o diretório do projeto com o comando
     `cd seu-repositorio`.
3. Crie um ambiente virtual utilizando o comando
     `python -m venv venv`.
4. Ative o ambiente virtual.
     Windows, use o comando `venv\Scripts\activate`
     MacOS/Linux, use o comando `source venv/bin/activate`.
5. Instale as dependências necessárias com o comando
    `pip install -r requirements.txt`.
6. Para iniciar o Jupyter Notebook, utilize o comando
    `jupyter notebook`.
7. No Jupyter Notebook, execute o notebook para coletar e analisar os dados das tarefas no Jira.
