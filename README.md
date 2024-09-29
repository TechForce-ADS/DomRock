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
        <td> Italo Bonilha </td>
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


<details> <summary> Clique aqui para ver a Sprint!</summary> 
  
## 🎯 Backlog da Sprint

| Rank | Prioridade | User Story                                                                                                                                                                                                                 | Sprint | Estimativa | Requisitos Relacionados          |
|------|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|------------|----------------------------------|
| 1    | Alta       | Como um representante da marca, eu quero que o sistema colete dados de reviews de produtos da base da B2W, para garantir que as informações sejam atualizadas e precisas.                                                 | 1      | 8          | RF1                              |
| 2    | Alta       | Como um representante da marca, eu quero que o sistema realize a limpeza de dados, eliminando duplicatas e corrigindo valores ausentes, para que eu tenha dados confiáveis para análise.                                   | 1      | 34          | RF1                               |
| 3    | Alta       | Como um representante da marca, eu quero que o sistema converta os reviews pré-processados em embeddings, para facilitar a recuperação de informações relevantes.                                                             | 1      | 8          | RF2                               |
| 4    | Média       | Como um representante da marca, eu quero visualizar a média de avaliação geral do produto solicitado para que eu possa ter uma visão clara do desempenho dos consumidores sobre a marca.                                  | 1      | 5          | RF6, RF4                          |
| 5    | Alta       | Como um representante da marca, eu quero identificar os produtos com as melhores e piores médias de avaliação para que eu possa direcionar ações de melhoria e destaque para os produtos.                                | 1      | 3          | RF6, RF4                          |
| 6  | Alta       | Como um representante da marca, eu quero que o sistema classifique os produtos com base em sentimentos extraídos dos reviews, para que eu possa entender melhor as motivações dos consumidores.                           | 1      | 8          | RF6                               |

## 📌 DOR - Definition of Ready

### 📄 User Stories e Critérios de Aceitação

#### US1: Como um representante da marca, eu quero que o sistema colete dados de reviews de produtos da base da B2W, para garantir que as informações sejam atualizadas e precisas.
Critérios de Aceitação:
- CA1: O sistema deve conectar-se à base da B2W e coletar os dados de reviews de produtos.
- CA2: Os dados coletados devem ser verificados para garantir que não estão desatualizados.
- CA3: O sistema deve informar ao usuário se a coleta foi bem-sucedida ou se houve algum erro.
  
#### US2: Como um representante da marca, eu quero que o sistema realize a limpeza de dados, eliminando duplicatas e corrigindo valores ausentes, para que eu tenha dados confiáveis para análise.
Critérios de Aceitação:
- CA1: O sistema deve identificar e remover duplicatas nos dados coletados.
- CA2: O sistema deve corrigir valores ausentes de forma adequada, utilizando regras definidas.
- CA3: O sistema deve gerar um relatório detalhando as ações de limpeza realizadas.
  
#### US3: Como um representante da marca, eu quero que o sistema converta os reviews pré-processados em embeddings, para facilitar a recuperação de informações relevantes.
Critérios de Aceitação:
- CA1: O sistema deve converter os reviews em embeddings utilizando técnicas de processamento de linguagem natural.
- CA2: Os embeddings devem ser armazenados em um banco de vetores (ex: ChromaDB ou FAISS).
- CA3: O sistema deve validar a integridade dos embeddings gerados.
  
#### US4: Como um representante da marca, eu quero visualizar a média de avaliação geral do produto solicitado para que eu possa ter uma visão clara do desempenho dos consumidores sobre a marca.
Critérios de Aceitação:
- CA1: O sistema deve permitir que o usuário faça perguntas sobre a média de avaliações de produtos específicos.
- CA2: O sistema deve buscar as avaliações do produto solicitado e calcular a média corretamente.
- CA3: A resposta deve ser apresentada em linguagem natural, indicando a média de avaliação do produto.

#### US5: Como um representante da marca, eu quero identificar os produtos com as melhores e piores médias de avaliação para que eu possa direcionar ações de melhoria e destaque para os produtos.
Critérios de Aceitação:
- CA1: O sistema deve entender perguntas sobre a identificação de produtos com melhores e piores médias de avaliação.
- CA2: O sistema deve calcular as médias de avaliação de todos os produtos disponíveis.
- CA3: A resposta deve apresentar os produtos com as melhores e piores médias de forma clara em linguagem natural.
  
#### US6: Como um representante da marca, eu quero que o sistema classifique os produtos com base em sentimentos extraídos dos reviews, para que eu possa entender melhor as motivações dos consumidores."
Critérios de Aceitação:
- CA1: Identificar produtos com maior e menor número de recomendações  
- CA2: Deve apresentar as razões por trás das recomendações de forma clara 
- CA3: O sistema deve permitir perguntas sobre produtos recomendados, com respostas claras e concisas
  
#### 🖼️ Wireframe

#### :cd: Dados 
Nessa entrega, usamos para a construção do chatbot com IA os dados do seguinte link:     
     https://huggingface.co/datasets/ruanchaves/b2w-reviews01


#### 🖥️ Entrega
</details>

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
#### RF1: Coleta e Processamento de Dados:
- O sistema deve coletar dados de reviews de produtos da base pública mencionada;
- O sistema deve realizar a limpeza de dados, eliminando duplicatas e corrigindo valores ausentes;
- O sistema deve realizar o pré-processamento dos reviews, extraindo e estruturando as informações para análise posterior.

#### RF2: Geração de Embeddings
- Os reviews pré-processados devem ser convertidos em embeddings, utilizando técnicas de processamento de linguagem natural;
- Os embeddings devem ser armazenados em um banco de vetores como ChromaDB ou FAISS para consulta eficiente.
  
#### RF3: Engenharia de Prompt
- Criar um agente que configure prompts otimizados para interação com LLM;
- Utilizar RAG (Retrieval Augmented Generation) para melhorar a qualidade das respostas, combinando recuperação de informações e geração de respostas.
  
#### RF4: Integração com Modelos LLM
- O sistema deve integrar-se com modelos de linguagem (por exemplo, GPT-2 ou T5) para processar as perguntas dos usuários.
- O sistema deve consultar o banco de vetores para recuperar informações relevantes e formular respostas adequadas.

#### RF5: Interface de Chatbot
- Criar uma interface de chatbot intuitiva e amigável para o usuário, utilizando Vue.js.
- O design da interface deve incluir botões de navegação claros e um layout limpo e organizado, garantindo uma experiência agradável.

#### RF6: Classificação de Produtos e Análise de Sentimentos
- O sistema deve classificar os produtos com base em sentimentos extraídos dos reviews, categorizando-os como:
     - Muito Bom (4-5)
     - Neutro (3)
     - Ruim (1-2)
- A classificação deve ser apresentada de maneira clara, permitindo que os usuários priorizem produtos mais bem avaliados e entendam as motivações por trás das notas.


### 🔨 Requisitos Não Funcionais (RNF)  
#### RNF 1: Teste e Avaliação
- O sistema deve permitir a realização de testes com diferentes modelos LLM e comparar suas respostas em termos de precisão e relevância;
- O sistema deve coletar feedback dos usuários para implementar melhorias futuras no chatbot.
  
#### RNF 2: Vídeo Tutorial
- O sistema deve incluir um vídeo tutorial que explique como usar a interface do chatbot, garantindo que os usuários tenham um suporte visual para maximizar a compreensão.

## :wrench: Metodologia  

  - Scrum

## :calendar: Calendário da Sprint
<img src="https://github.com/TechForce-ADS/imagens/blob/main/2.png" width="800px"> 


## :page_with_curl: Backlog do Produto

| Rank | Prioridade | User Story                                                                                                                                                                                                                 | Sprint | Estimativa | Requisitos Relacionados          |
|------|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------|------------|----------------------------------|
| 1    | Alta       | Como um representante da marca, eu quero que o sistema colete dados de reviews de produtos da base da B2W, para garantir que as informações sejam atualizadas e precisas.                                                 | 1      | 8          | RF1                              |
| 2    | Alta       | Como um representante da marca, eu quero que o sistema realize a limpeza de dados, eliminando duplicatas e corrigindo valores ausentes, para que eu tenha dados confiáveis para análise.                                   | 1      | 34          | RF1                               |
| 3    | Alta       | Como um representante da marca, eu quero que o sistema converta os reviews pré-processados em embeddings, para facilitar a recuperação de informações relevantes.                                                             | 1      | 8          | RF2                               |
| 4    | Média       | Como um representante da marca, eu quero visualizar a média de avaliação geral do produto solicitado para que eu possa ter uma visão clara do desempenho dos consumidores sobre a marca.                                  | 1      | 5          | RF6, RF4                          |
| 5    | Alta       | Como um representante da marca, eu quero identificar os produtos com as melhores e piores médias de avaliação para que eu possa direcionar ações de melhoria e destaque para os produtos.                                | 1      | 3          | RF6, RF4                          |
| 6  | Alta       | Como um representante da marca, eu quero que o sistema classifique os produtos com base em sentimentos extraídos dos reviews, para que eu possa entender melhor as motivações dos consumidores.                           | 1      | 8          | RF6                               |
| 7    | Média       | Como um representante da marca, eu quero saber quais produtos são mais e menos recomendados pelos consumidores para que eu possa entender os motivos por trás dessas avaliações e tomar decisões estratégicas.          | 2      | 34          | RF4, RF6                          |
| 8    | Média       | Como um representante da marca, eu quero analisar os comentários mais frequentes sobre os produtos, para que eu possa identificar padrões problemáticos recorrentes e pontos fortes dos produtos.                          | 2      | 21          | RF1, RF4                          |
| 9    | Baixa       | Como um representante da marca, eu quero entender a relação entre as avaliações e as características demográficas dos consumidores (idade, sexo, região) para que eu possa personalizar as campanhas de venda e desenvolvimento dos produtos. | 2      | 2          | RF4                               |
| 10    | Baixa       | Como um representante da marca, eu quero que o sistema tenha uma interface de chatbot intuitiva e amigável, para que eu consiga interagir facilmente com a ferramenta.                                                      | 2      | 8          | RF5                               |
| 11   | Baixa      | Como um representante da marca, eu quero um vídeo tutorial explicando como usar o chatbot, para que eu possa entender melhor a funcionalidade e utilizar a ferramenta de forma eficaz.                                    | 3      | 1         | RNF2                               |
| 12   | Média      | Como um representante da marca, eu quero que o sistema permita a comparação entre diferentes modelos LLM em termos de precisão e relevância das respostas, para garantir a melhor experiência possível.                   | 3      | 21          | RNF1                               |



## :computer: Tecnologias Utilizadas 
Essas foram as tecnologias usadas no nosso projeto:

<img src="https://github.com/TechForce-ADS/imagens/blob/main/1.png" width="800px"> 

  - Python
  - Jupyter Notebook
  - Trello
  - VS Code
  - GitHub


## :triangular_ruler: Padronização de Commits
Padronização dos commits: < Sprint X> < tipo>: <descrição breve da tarefa>

- < Sprint X>: Refere-se ao número da sprint em que a mudança foi implementada. 
- < tipo>: Indica o tipo de mudança realizada. 
- < descrição>: Uma breve descrição da mudança realizada. 

 Exemplo: < Sprint I> < fix>: <Correção de bugs>

## :books: Sprint
- >  <a href="https://github.com/TechForce-ADS/DomRock/tree/main/Sprint1"> 1° Sprint
 

