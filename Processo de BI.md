
**Data:** 2025-03-15
**keyboards:** 
**links internos:** 
___

# Processo de Dados BI

Existem cinco 5 Etapas no processo de Dados em BI. São elas: 

![[Pasted image 20250315105410.png]]


## *ETL (Extrair, Transformar e Carregar)*


1. **EXTRAÇÃO**: 

- Nesta etapa, os Dados são Coletados de diversas fontes, que podem incluir bancos de dados, arquivos de texto, planilhas, Sistemas CRM, entre outros.
- O objetivo é reunir todos os dados relevantes para a análise em um único local


2. **TRANSFORMAÇÃO**:

- Os dados extraídos geralmente estão em formato diferentes e podem conter erros ou inconsistências
- Na etapa de transformação, os dados são limpos, padronizados, organizados e enriquecidos para garantir sua qualidade e consistência.

- Isso pode incluir tarefas como:

	- Remoção de dados duplicados ou irrelevantes.
	- Correção de erros de digitação ou formatação.
	- Conversão de dados para um formato padrão.
	- Cálculo de novos campos ou métricas.
	- Agregação de dados.


3. **CARREGAMENTO**:

-  Após a transformação, os dados são carregados em um sistema de armazenamento der Dados, como um Power BI ou warehouse

- Esse sistema é otimizado para análise e permite que os usuários acessem os dados de forma rápida e eficiente.

## *Modelagem de dados*


**1. Criação de Relacionamentos:**

- **Conexão entre Tabelas:**
    - Em um ambiente de BI, os dados geralmente são armazenados em várias tabelas diferentes. A criação de relacionamentos estabelece conexões entre essas tabelas, permitindo que os dados sejam combinados e analisados de forma integrada.
- **Chaves Primárias e Estrangeiras:**
    - Os relacionamentos são criados com base em chaves primárias (identificadores únicos em uma tabela) e chaves estrangeiras (referências a chaves primárias em outras tabelas). Isso garante a integridade e a consistência dos dados.
- **Tipos de Relacionamentos:**
    - Existem diferentes tipos de relacionamentos, como um-para-um, um-para-muitos e muitos-para-muitos. A escolha do tipo correto de relacionamento é fundamental para garantir a precisão das análises.
- **Importância:**
    - A criação de relacionamentos permite que os usuários explorem os dados de forma mais profunda, identificando padrões e tendências que não seriam visíveis em tabelas isoladas.


**2. MODELAGEM DE DADOS:**

- **Estruturação dos Dados:**
    - A modelagem de dados envolve a organização e a estruturação dos dados em um formato que seja adequado para análise. Isso inclui a definição de tabelas, colunas, relacionamentos e outras estruturas de dados.
- **Modelos Dimensionais:**
    - Em muitos casos, os dados de BI são modelados usando modelos dimensionais, como o modelo estrela ou o modelo floco de neve. Esses modelos facilitam a análise de dados por meio da separação de dados em fatos (medidas) e dimensões (atributos).
- **Otimização para Análise:**
    - A modelagem de dados visa otimizar o desempenho das consultas e análises, garantindo que os usuários possam acessar as informações de forma rápida e eficiente.
- **Importância:**
    - Uma modelagem de dados bem feita é essencial para garantir a qualidade, a consistência e a usabilidade dos dados em um ambiente de BI. Ela permite que os usuários criem relatórios e dashboards precisos e relevantes, que auxiliam na tomada de decisões estratégicas.


**Em resumo:**

- A criação de relacionamentos conecta as tabelas de dados, permitindo a análise integrada.
- A modelagem de dados estrutura os dados de forma otimizada para análise, facilitando a criação de relatórios e dashboards.

Juntas, essas etapas são fundamentais para transformar dados brutos em informações valiosas para o BI.


## *Cálculos/Análises*


**Cálculos e Análises no BI:**

- **Objetivo:**
    - O objetivo principal dos cálculos e análises no BI é extrair informações valiosas dos dados, identificar padrões, tendências e anomalias, e fornecer suporte para a tomada de decisões estratégicas.
- **Tipos de Cálculos:**
    - Os cálculos podem variar desde operações simples, como somas, médias e contagens, até análises mais complexas, como previsões, análises de tendências e modelagem estatística.
- **Ferramentas:**
    - As ferramentas de BI, como o Power BI, o Tableau e o QlikView, oferecem uma ampla gama de funções e recursos para a criação de cálculos e análises.

**Análises com Fórmulas DAX:**

- **O que é DAX?**
    - DAX é uma linguagem de fórmulas e expressões usada em ferramentas de análise de dados da Microsoft, como o Power BI, o Analysis Services e o Power Pivot no Excel.
    - Ela permite criar cálculos personalizados, colunas calculadas e medidas para análises de dados avançadas.
- **Capacidades do DAX:**
    - O DAX oferece uma ampla gama de funções para realizar cálculos complexos, incluindo:
        - Funções de agregação (SUM, AVERAGE, COUNT).
        - Funções de data e hora.
        - Funções lógicas.
        - Funções de filtro.
        - funções financeiras.
- **Aplicações do DAX:**
    - O DAX é amplamente utilizado para:
        - Criar medidas personalizadas para calcular métricas de desempenho.
        - Realizar análises de tendências e previsões.
        - Criar relatórios e dashboards interativos.
        - Realizar comparações entre períodos.


**Importância dos Cálculos e Análises com DAX:**

- **Personalização:**
    - O DAX permite criar cálculos personalizados que atendem às necessidades específicas de cada análise.
- **Flexibilidade:**
    - O DAX oferece uma grande flexibilidade para realizar análises complexas e explorar os dados de diferentes perspectivas.
- **Insights Profundos:**
    - O DAX permite extrair insights mais profundos dos dados, revelando padrões e tendências que não seriam visíveis com cálculos simples.

Em resumo, os cálculos e análises, especialmente com o uso de fórmulas DAX, são essenciais para transformar dados brutos em informações valiosas e acionáveis no contexto do BI.


## *Criação de Dashboards*


**Principais características e objetivos dos dashboards:**

- **Visualização de dados:**
    - Os dashboards utilizam gráficos, tabelas e outros elementos visuais para apresentar os dados de forma clara e intuitiva.
- **Monitoramento de KPIs:**
    - Eles permitem acompanhar os indicadores-chave de desempenho, como vendas, receita, custos, entre outros, em tempo real ou em intervalos regulares.
- **Tomada de decisões:**
    - Os dashboards fornecem informações relevantes para auxiliar na tomada de decisões estratégicas e operacionais.
- **Interatividade:**
    - Muitos dashboards são interativos, permitindo que os usuários explorem os dados, filtrem informações e façam análises detalhadas.
- **Personalização:**
    - É possível personalizar os dashboards para atender às necessidades específicas de cada usuário ou departamento.

**Processo de criação de dashboards:**

1. **Definição dos objetivos:**
    - É importante definir claramente quais informações serão apresentadas no dashboard e qual o objetivo da análise.
2. **Seleção dos KPIs:**
    - Escolher os indicadores-chave de desempenho mais relevantes para o negócio.
3. **Escolha das visualizações:**
    - Selecionar os tipos de gráficos e tabelas mais adequados para apresentar os dados.
4. **Design do dashboard:**
    - Criar um layout organizado e visualmente atraente, facilitando a leitura e a interpretação dos dados.