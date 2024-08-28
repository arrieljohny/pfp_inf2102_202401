# Projeto: Análise de Sentimentos e Gestão de Tarefas com Jira

## Descrição

Este projeto é um software desenvolvido em Python e organizado na plataforma Jupyter Notebook com o objetivo de coletar informações de tarefas do software de apoio à gestão de projetos Jira. O software extrai dados sobre responsáveis, tempo estimado e tempo gasto em cada tarefa. Além disso, analisa os textos descritos nas descrições e comentários das tarefas para classificar os sentimentos presentes no conteúdo textual.

## Visão de Projeto

### Cenários de Uso Positivos

1. **Identificação de Tendências de Produtividade**:
   **Usuário:** Gestor de projetos com familiaridade em liguagem de programação python
   **Contexto:** Gostaria de analisar a tendência de produtividade e assertividade no planejamento
   **Narrativa:** Coleta e analisa dados das tarefas planejadas e concluidas em um conjunto de sprints verificando se a equipe está consistentemente cumprindo os prazos e entregando tarefas dentro do tempo estimado. Esse cenário positivo permite à gestão identificar boas práticas e replicá-las em outras equipes, promovendo a eficiência em toda a organização.

2. **Melhoria no Clima Organizacional**:
   **Usuário:** Gestor de projetos com familiaridade em liguagem de programação python
   **Contexto:** Gostaria de analisar o clima organizacional através das comunicações realizadas nas tarefas da equipe
   **Narrativa:** Coleta dados textuais das tarefas e analisa os sentimentos expressos nas descrições e comentários das tarefas, a ferramenta pode identificar um aumento nos sentimentos positivos, como "Happy" e "Surprise", após a implementação de novas políticas de bem-estar no ambiente de trabalho. Esse feedback possibilita à empresa entender que suas ações estão impactando positivamente o moral e a motivação dos funcionários.

### Cenários de Uso Negativos

1. **Detecção de Burnout**:
   A análise de sentimentos revela um aumento significativo em sentimentos negativos, como "Sad" e "Fear", nos comentários de determinadas equipes, especialmente em tarefas com prazos apertados. Esse cenário negativo pode indicar sinais de burnout ou estresse elevado entre os membros da equipe, alertando a gestão para a necessidade de intervenções, como reavaliação de cargas de trabalho ou suporte adicional.

2. **Atrasos e Ineficiências Repetidas**:
   Os dados mostram que certas tarefas repetidamente excedem o tempo estimado, com responsáveis frequentemente reportando dificuldades ou obstáculos. Além disso, a análise de sentimentos aponta para frustração e insatisfação nesses comentários. Este cenário negativo evidencia possíveis gargalos no processo ou problemas na alocação de recursos, exigindo uma revisão detalhada das causas para evitar prejuízos futuros.


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
  `deep_translator`

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
