# Projeto: Análise de Sentimentos e Gestão de Tarefas com Jira

## Descrição

Este projeto é um software desenvolvido em Python e organizado na plataforma Jupyter Notebook com o objetivo de coletar informações de tarefas do software de apoio à gestão de projetos Jira. O sistema extrai dados sobre responsáveis, tempo estimado e tempo gasto em cada tarefa. Além disso, analisa os textos descritos nas descrições e comentários das tarefas para classificar os sentimentos presentes no conteúdo textual.

## Funcionalidades

### Coleta de Dados

- **Conexão com a API do Jira**: O sistema se conecta à API do Jira para coletar informações sobre tarefas.
- **Extração de Dados**: Coleta de dados como responsáveis, tempo estimado e tempo gasto em cada tarefa.

### Análise de Sentimentos

- **Análise de Textos**: O sistema realiza uma análise dos textos presentes nas descrições e comentários das tarefas.
- **Classificação de Sentimentos**: Utilização da biblioteca `text2emotion` para classificar os sentimentos expressos nos textos em cinco categorias: *Happy*, *Angry*, *Surprise*, *Sad*, e *Fear*.

## Requisitos

- Python 3.0+
- Jupyter Notebook
- Bibliotecas
  `text2emotion`
  `requests`
  `customtkinter`
  `tkinter`
  `json`
  `os` 
  `dotenv`
  `urllib.parse`
  `pandas` 

## Instalação

1. Clone este repositório:

   ```bash
   git clone https://github.com/arrieljohny/pfp_inf2102_202401.git

2. Navegue até o diretório do projeto com o comando
   ```bash
   `cd seu-repositorio`

3. Crie um ambiente virtual utilizando o comando
   ```bash
   `python -m venv venv`
   
4. Ative o ambiente virtual no Windows | MacOS/Linux
   ```bash
   `venv\Scripts\activate`

   `source venv/bin/activate`
   
5. Instale as dependências necessárias com o comando
   ```bash
   `pip install -r requirements.txt`.

6. Para iniciar o Jupyter Notebook, utilize o comando
   ```bash
   `jupyter notebook`.
   
7. No Jupyter Notebook, execute o notebook para coletar e analisar os dados das tarefas no Jira.
