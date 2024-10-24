# DomRock
Este repositório é dedicado ao desenvolvimento da API para o 6º semestre, em colaboração com a Dom Rock.

<br>
<table>
  <tr>
    <td>Cliente</td>
    <td>Periodo/Curso</td>
    <td>Professor M2</td>
    <td>Professor P2</td>
  </tr>
  <tr>
    <td> Dom Rock</td>
    <td> 6º ADS (Análise e Desenvolvimento de Sistemas) </td>
    <td> Eduardo Sakaue </td>
    <td> Walmir Duque  </td>
  </tr>
</table>
</br>


# Equipes
 <table align="center" border="1">
    <tr>
        <td>SCRUM MASTER</td>
        <td>PRODUCT OWNER</td>
        <td>SCRUM TEAM</td>
        <td>SCRUM TEAM</td>
        <td>SCRUM TEAM</td>
        <td>SCRUM TEAM</td>
        <td>SCRUM TEAM</td>
        <td>SCRUM TEAM</td>
        <td>SCRUM TEAM</td>
  <tr>
        <td> Debora Taira</td>
        <td> Ítalo Bonilha </td>
        <td> Brener Freire </td>
        <td> Francisco Quirino </td>
        <td> Gabriel Angelis</td>
        <td> Isabel Reis </td>
        <td> Pedro Seraggi </td>
        <td> Renato Passos </td>
        <td> Roberta Cristina</td>


</table>

 
## :pencil: Projeto 
Desenvolver um chatbot baseado em IA generativa que possa receber perguntas, buscar respostas na base de dados de comentários de clientes e apresentar essas respostas em linguagem natural. Através dessa solução, os representantes de marcas poderão acessar rapidamente o feedback dos consumidores, obtendo uma visão clara e detalhada sobre como seus produtos estão sendo avaliados.

Com base na análise dos dados e na proposta do projeto, o foco está na consultoria de dados para os representantes de marca. Isso permitirá que esses profissionais acompanhem a percepção do consumidor em relação a seus produtos, auxiliando na criação de estratégias de vendas mais eficazes e assertivas. O chatbot também permitirá a identificação de padrões e tendências nas avaliações, oferecendo insights úteis para melhorias contínuas.


## :books: Sprint
- >  <a href="https://github.com/TechForce-ADS/DomRock/tree/main/Sprint1"> 1° Sprint
 


  ## :blue_book: Conhecimentos do Semestre  
Abaixo estão os conhecimentos aplicados durante o nosso semestre:
  - Implementar Aplicação usando SpringBoot e características técnicas mais avançadas
  - Implementar FrontEnd SPA (Single Page Application) com Vue.js
  - Desenvolver Aplicação em Machine Learning, com base no modelo CRISP, utilizando paradigma Supervisionado ou Não Supervisionado
  - Linguagem Java Web Server-Side
  - Framework SpringBoot
  - Linguagem Python (IA / Machine Learning)
  - Biblioteca SKLearn (IA / Machine Learning)
  - BibliotecaTensor Flow / Keras (IA / Deep Learning)
    
 ## :white_check_mark: Requisitos  
### :clipboard: Requisitos Funcionais (RF)
#### RF1: Perguntas sobre detalhes dos produtos, (como qualidade, performance, eficiência etc.) 
  - O sistema deve permitir que os representantes da marca façam perguntas sobre os produtos com base em reviews e notas gerais da base de dados B2W e forneça respostas em linguagem natural.

#### RF2: Estatística de avaliações de produtos alocados em rankigs ou tabela: 
  - O sistema deve calcular médias de avaliações e gerar rankings ordenados para facilitar a comparação entre produtos da mesma categoria.

#### RF3: Análise de sentimento dos produtos identificando se o produto tem suas reviews avaliadas em sua maioria como positivas neutras ou negativas: 
  - O sistema deve classificar as reviews dos produtos em sentimentos (positivo, neutro, negativo) e gerar um resumo textual explicando a classificação.

#### RF4: Análise de Padrões, Consulta de defeitos encontrados em um dado produto 
  - O sistema deve identificar padrões nas reviews (palavras e frases-chave recorrentes) e associar termos relevantes para gerar um resumo dos problemas mais comuns. 

#### RF5: Análise de consumo de produtos por característica demográfica (idade, sexo, região, por ex.) 
  - O sistema deve correlacionar as avaliações com dados demográficos dos consumidores (idade, sexo, região) e gerar relatórios que expliquem as preferências de diferentes segmentos de público.

#### RF6: Recomendação de produtos baseado no interesse do usuário
  - O sistema deve permitir que os representantes da marca façam perguntas sobre os produtos presentes na base de dados da B2W e com base nas reviews e notas gerais gere recomendações de acordo com seu interesse.

 

### 🔨 Requisitos Não Funcionais (RNF)   

#### RNF1: BD Vetorial ChromaDB, FAISS ou outro
  - Utilização do FAISS para armazenar e consultar informações.

#### RNF2: Integração com interface visual
  - Integração entre o sistema de backend (processamento de dados, análise de sentimentos, rankings, etc.) e uma interface visual
  
 #### RNF3: Teste com modelos LLM de uso público do Huggingface
  - O sistema deve ser testado com modelos LLM de uso público, como os disponibilizados no Huggingface.
    
 #### RNF4: Framework Langchain
 - Implementar o framework Langchain para lidar com consultas em linguagem natural e análise de dados.
   
 #### RNF4: Vídeo-tutorial;
- Incluir um vídeo-tutorial para guiar os usuários na utilização do sistema.
  
## :wrench: Metodologia  

  - Scrum

## :calendar: Calendário da Sprint
<img src="https://github.com/TechForce-ADS/imagens/blob/main/2.png" width="800px"> 


## :page_with_curl: Backlog do Produto

| Rank | Prioridade | User Story       | Sprint | Estimativa | Requisitos Relacionados          |
|------|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|------------|----------------------------------|
| 1    | Alta       | Desenvolvimento RAG/ ChromaDB, Como um representante da marca eu quero conseguir fazer perguntas sobre os produtos disponíveis na base de dados da B2W e com base nas reviews e notas gerais obter recomendações de acordo com o interesse do usuário em linguagem natural.                                                | 1      | 34          | RF6, RF1, RNF1, RNF3, RNF4                              |
| 2    | Alta       | Desenvolvimento RAG/ ChromaDB, Como um representante da marca eu quero conseguir fazer perguntas sobre os detalhes (qualidade, performance, eficiência etc) dos produtos disponíveis na base de dados da B2W e obter respostas em linguagem natural.                                                | 2      | 34          | RF1, RNF1, RNF3, RNF4                              |
| 3    | Alta       | Integração com a base de dados/ Criação de Ranking com base nas avaliações, Como um representante da marca eu quero visualizar as médias de avaliação dos produtos disponíveis na base de dados da B2W e gerar rankings crescentes e decrescentes usando parâmetros como média geral, sentimentos, e atributos.                                   | 2      | 34         | RF2, RF3, RNF1, RNF3, RNF4                               |
| 4    | Alta       | Integração com a base de dados/ Análise de sentimento das reviews, Como um representante da marca eu quero saber quais produtos são mais e menos recomendados, identificando os sentimentos das reviews (positivo, neutro, negativo), para entender melhor as motivações dos consumidores.                                                       | 2      | 22         | RF3, RNF1, RNF3, RNF4                               |
| 5    | Alta       | Análise de padrões e satisfação do cliente, Como um representante da marca eu quero poder identificar padrões nas reviews sobre os produtos a fim de encontrar problemas recorrentes.                           | 2      | 22          | RF4, RNF1, RNF3, RNF4                          |
| 6  | Média       | Análise demográfica, Como um representante da marca eu quero entender a relação entre as avaliações e as características demográficas dos consumidores para poder personalizar minhas ações de vendas com base nas preferências e características de diferentes segmentos de público-alvo.                   | 2      | 22          | RF5, RNF1, RNF3, RNF4                               |
| 7    | Baixa       | Usabilidade, Como um representante da marca e usuário final, eu quero que o sistema tenha uma interface visual intuitiva e amigável, para que eu consiga interagir facilmente com os dados e análises realizadas.         | 3      | 12          | RF1, RNF2                        |                            |
| 8    | Baixa       | Tutorial para o usuário, Como um representante da marca eu quero um vídeo tutorial explicando como usar o chatbot, para que eu possa entender melhor a funcionalidade e utilizar a ferramenta de forma eficaz.                                                      | 3      | 2          | RNF5                               |
                                                                                                                                                                                                             


## :computer: Tecnologias Utilizadas 
Essas foram as tecnologias usadas no nosso projeto:

<img src="https://github.com/TechForce-ADS/imagens/blob/main/Tecnologias%20Utilizadas.png" width="800px"> 

  - Python
  - Jupyter Notebook
  - Jira
  - VS Code
  - GitHub


## :triangular_ruler: Padronização de Commits
Padronização dos commits: < Sprint X> < tipo>: <descrição breve da tarefa>

- < Sprint X>: Refere-se ao número da sprint em que a mudança foi implementada. 
- < tipo>: Indica o tipo de mudança realizada. 
- < descrição>: Uma breve descrição da mudança realizada. 

 Exemplo: < Sprint I> < fix>: <Correção de bugs>


