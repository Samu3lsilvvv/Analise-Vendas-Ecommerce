# <font color='blue'>Análise Exploratória de Vendas Para Loja de E-commerce</font>

### Visão Geral do Projeto
Este projeto consiste em uma Análise Exploratória de Dados (EDA) completa sobre um conjunto de dados simulado de transações de vendas de uma loja de e-commerce. O objetivo principal é extrair insights estratégicos e acionáveis dos dados brutos, transformando-os em recomendações de negócio para otimizar o portfólio de produtos, a estratégia de marketing e a logística.

O desenvolvimento foi realizado em Python utilizando o ambiente Jupyter Notebook, que permite uma abordagem passo a passo e visual para a análise de dados.

A análise foi estruturada para responder às seguintes perguntas-chave:

1.  **Performance de Produtos:** Quais são os produtos mais populares em termos de volume de vendas?
2.  **Tendências de Faturamento:** Como o faturamento evoluiu ao longo do tempo (mensalmente), permitindo a identificação de sazonalidades e tendências?
3.  **Foco Regional:** Qual a distribuição geográfica das vendas e quais são os mercados estaduais mais fortes?
4.  **Otimização de Portfólio:** Quais categorias de produtos geram a maior receita para a empresa?


### Tecnologias e Bibliotecas

O projeto foi desenvolvido em **Python** no ambiente **Jupyter Notebook**. As bibliotecas utilizadas são:

* **Pandas:** Para manipulação, limpeza e pré-processamento dos dados.
* **NumPy:** Utilizado para operações numéricas.
* **Matplotlib e Seaborn:** Para a criação e personalização de visualizações de dados.

### Metodologia e Estrutura do Notebook
O notebook DSA-Python-MiniProjeto1.ipynb está organizado em seções que refletem o fluxo de trabalho padrão de um projeto de Data Science:

**Preparação dos Dados**

• Geração de Dados Fictícios: Uma função personalizada (gerador_dados_ficticios) é usada para criar um DataFrame simulado que representa as transações de vendas, garantindo que o projeto seja totalmente auto-suficiente e replicável.

• Inspeção e Limpeza Inicial: Verificação de tipos de dados (dtypes), contagem de valores nulos e validação da estrutura das colunas.

**Engenharia de Variáveis**

• Criação de novas variáveis para a análise:

• Valor_Total_Venda: Calculado a partir de Preco_Unitario * Quantidade.

• Mês_Pedido: Extração do mês da coluna Data_Pedido para análise de sazonalidade.

**Análise Exploratória de Dados**

Esta seção é o cerne do projeto, onde o Pandas é usado para responder às questões de negócio através de agregações e visualizações.

### Principais Questões de Negócio e Insights

##### A. Performance de Produtos (O que é mais vendido?)

**Questão:** Quais são os Top 10 produtos mais vendidos?

**Análise Realizada:** Agregação por Nome_Produto e soma de Quantidade

##### B. Otimização de Portfólio (Onde está o dinheiro?)

**Questão:** Qual categoria gera mais receita?

**Análise Realizada:** Agregação por Categoria e soma de Valor_Total_Venda.

##### C. Tendências e Sazonalidade (Quando devemos investir?)

**Questão:** Como o faturamento evoluiu ao longo do tempo?

**Análise Realizada:** Agregação mensal do Valor_Total_Venda e visualização em gráfico de linha.

##### D. Foco Regional (Para onde expandir?)

**Questão:** Qual estado tem o maior faturamento?

**Análise Realizada:** Agregação por Estado e soma de Valor_Total_Venda (Top 5).



