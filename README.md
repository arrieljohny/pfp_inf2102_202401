# Projeto: Análise de Sentimentos e Gestão de Tarefas com Jira

## Descrição

Este projeto é um software desenvolvido em Python e organizado na plataforma Jupyter Notebook com o objetivo de coletar informações de tarefas do software de apoio à gestão de projetos Jira. O software extrai dados sobre responsáveis, tempo estimado e tempo gasto em cada tarefa. Além disso, analisa os textos descritos nas descrições e comentários das tarefas para classificar os sentimentos presentes no conteúdo textual.

## Visão de Projeto  

### Cenários de Uso Positivos  

1. **Identificação de Tendências de Produtividade**:

   **Usuário:** Gestor de projetos com familiaridade em liguagem de programação python.
   
   **Contexto:** Gostaria de analisar a tendência de produtividade e assertividade no planejamento.  

   **Narrativa:** Coleta e analisa dados das tarefas planejadas e concluidas em um conjunto de sprints verificando se a equipe está consistentemente cumprindo os prazos e entregando tarefas dentro do tempo estimado. Esse cenário positivo permite à gestão identificar boas práticas e replicá-las em outras equipes, promovendo a eficiência em toda a organização.  

2. **Melhoria no Clima Organizacional**:  

   **Usuário:** Gestor de projetos com familiaridade em liguagem de programação python.  

   **Contexto:** Gostaria de analisar o clima organizacional através das comunicações realizadas nas tarefas da equipe.  

   **Narrativa:** Coleta dados textuais das tarefas e analisa os sentimentos expressos nas descrições e comentários das tarefas, a ferramenta pode identificar um aumento nos sentimentos positivos, como "Happy" e "Surprise", após a implementação de novas políticas de bem-estar no ambiente de trabalho. Esse feedback possibilita à empresa entender que suas ações estão impactando positivamente o moral e a motivação dos funcionários.

3. **Detecção de Burnout**:  

   **Usuário:** Gestor de projetos ou gestor de recursos humanos com familiaridade em liguagem de programação python.  

   **Contexto:** Gostaria de realizar uma possivel detecção de burnout através das comunicações realizadas nas tarefas da equipe.  

   **Narrativa:** Coleta dados textuais das tarefas e a análise de sentimentos revela um aumento significativo em sentimentos negativos, como "Sad" e "Fear", nos comentários de determinadas equipes, especialmente em tarefas com prazos apertados. Esse cenário negativo pode indicar sinais de burnout ou estresse elevado entre os membros da equipe, alertando a gestão para a necessidade de intervenções, como reavaliação de cargas de trabalho ou suporte adicional.  

### Cenários de Uso Negativos  

1. **Falta de Conhecimento em Liguagem de Programação Python**:  
   O software presume que o usuário tenha familiaridade com a linguagem Python para realizar as adaptações necessárias à reutilização do código. Portanto, um cenário problemático seria a tentativa de uso por parte de alguém sem esse conhecimento técnico, o que poderia comprometer a eficácia do software. Além disso, o software opera inteiramente via código, sem oferecer uma interface gráfica para facilitar a interação.

2. **Preenchimento Inadequado das Tarefas no Jira**:  
   O software realiza a mineração e analise de dados da plataforma Jira. No entanto, se os dados não forem corretamente preenchidos, as analises pode apresentar resultados inconsistentes com a realidade do projeto.

##Documentação Técnica do Projeto

### Requisitos Funcionais

1. **Coleta de Dados do Jira**:
   - O software deve se conectar à API do Jira e extrair informações detalhadas sobre as tarefas.
   - O software deve ser capaz de autenticar-se na API do Jira utilizando as credenciais fornecidas pelo usuário.

2. **Análise de Sentimentos**:
   - O software deve analisar os textos presentes nas descrições e comentários das tarefas, identificando e classificando os sentimentos expressos.
   - A classificação dos sentimentos deve ser realizada em cinco categorias: Happy, Angry, Surprise, Sad, e Fear, utilizando a biblioteca `text2emotion`.

3. **Configuração e Personalização**:
   - O software deve permitir que o usuário selecione os tipos de itens a serem minerados e analisados, como tarefas, histórias de usuários, épicos, dentre outros disponíveis no projeto.

### Requisitos Não Funcionais

1. **Desempenho**:
   - O software deve ser capaz de processar e analisar grandes volumes de dados provenientes do Jira sem comprometimento significativo do desempenho.
   - O tempo de resposta para a coleta e análise de dados deve ser minimizado para garantir a eficiência.

2. **Escalabilidade**:
   - O software deve ser escalável para acomodar o crescimento no volume de tarefas e projetos gerenciados pelo Jira, sem necessidade de reestruturação significativa.

3. **Manutenibilidade**:
   - O código do software deve ser bem documentado e modular, facilitando futuras manutenções, atualizações e adaptações.

4. **Usabilidade**:
   - Embora o software não possua uma interface gráfica, ele deve ser estruturado de forma clara e acessível para desenvolvedores, com instruções detalhadas para sua configuração e uso.

## Manual de Utilização

### Introdução

Este manual tem como objetivo orientar o usuário na utilização do software desenvolvido para a coleta e análise de dados de tarefas gerenciadas pela plataforma Jira. 

O software foi concebido para auxiliar equipes de projeto e gestores na obtenção de insights valiosos sobre a eficiência do trabalho e o bem-estar das equipes. Através da integração com a API do Jira, o sistema coleta informações detalhadas sobre tarefas, como responsáveis, tempo estimado e tempo gasto. Além disso, o software realiza uma análise de sentimentos nos textos das descrições e comentários das tarefas, utilizando a biblioteca `text2emotion` para identificar emoções como felicidade, raiva, surpresa, tristeza e medo.

Com esses dados, o sistema visa fornecer uma visão clara e objetiva do andamento dos projetos e do clima organizacional, permitindo uma gestão mais informada e proativa. Este manual descreve as funcionalidades, os requisitos, e as instruções de uso do software, garantindo que o usuário possa aproveitar ao máximo suas capacidades.


### **Funcionalidades**

### Coleta de Dados

- **Conexão com a API do Jira**: O software se conecta à API do Jira para coletar informações sobre tarefas.
- **Extração de Dados**: Coleta de dados como responsáveis, tempo estimado e tempo gasto em cada tarefa.

### Análise de Sentimentos

- **Análise de Textos**: O software realiza uma análise dos textos presentes nas descrições e comentários das tarefas.
- **Classificação de Sentimentos**: Utilização da biblioteca `text2emotion` para classificar os sentimentos expressos nos textos em cinco categorias: *Happy*, *Angry*, *Surprise*, *Sad*, e *Fear*.

### Requisitos

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

### Instalação

### Instalação do Jupyter Notebook

Para instalar o Jupyter Notebook, siga os passos abaixo:

1. Instale o Python
Caso ainda não tenha o Python instalado, faça o download e instale a versão mais recente do Python 3.x a partir do [site oficial do Python](https://www.python.org/downloads/). Durante a instalação, certifique-se de marcar a opção "Add Python to PATH".

2. Atualize o pip
Abra o terminal (Prompt de Comando no Windows, Terminal no macOS/Linux) e atualize o `pip`, o gerenciador de pacotes do Python:  
  ```bash
  python -m pip install --upgrade pip
