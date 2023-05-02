# O que é um data warehouse?
Primeiro, vamos definir o que é um data warehouse e por que você pode querer usar um para sua organização.

Um data warehouse é um repositório centralizado que armazena dados estruturados (tabelas de banco de dados, planilhas do Excel) e dados semiestruturados (arquivos XML, páginas da Web) para fins de relatório e análise. Os dados fluem de uma variedade de fontes, como sistemas de ponto de venda, aplicativos de negócios e bancos de dados relacionais, e geralmente são limpos e padronizados antes de chegar ao depósito. Como um data warehouse pode armazenar grandes quantidades de informações, ele fornece aos usuários acesso fácil a uma grande quantidade de dados históricos, que podem ser usados para mineração de dados, visualização de dados e outras formas de relatórios de business intelligence.

# Conceito de Data Warehouse
O Data Warehouse é um armazém de dados ou repositório de dados. Trata-se de uma estrutura de armazenamento que guarda dados em um formato estruturado para facilitar consultas e análises. Não é somente um conjunto de dados, mas um conjunto disposto para facilitar o uso por ferramentas analíticas.

Nesse sentido, um warehouse se destaca como uma opção para coleta e tratamento do Big Data. Além disso, é uma importante ferramenta para projetos de Data Science, servindo como uma base estrutural com dados para treinamento de algoritmos.

Em suma, o DW registra os dados e os históricos associados para possibilitar a melhor tomada de decisão de gestores. Dessa forma, permite responder a perguntas importantes do negócio, como quantas vendas foram feitas no mês X, quantos clientes desistiram do serviço no mês passado e outras questões relacionadas.

O time de marketing, por exemplo, pode olhar para dados de acesso do site e do blog para pensar em abordagens de SEO ou melhorias consideráveis na personalização do conteúdo. O marketing de conteúdo e o email marketing também são favorecidos com o uso do warehouse como um repositório central de dados, uma vez que é possível o ajuste das estratégias constantemente.

# Conheça a arquitetura de um Data Warehouse
Vamos aprofundar no conceito de um DW. Agora, falaremos sobre a arquitetura que compõe essa estrutura.

Inicialmente, vale destacar que a arquitetura varia muito a depender da robustez e complexidade do DW. Os elementos que citaremos a seguir são organizados em camadas que realizam algum tipo de função, sendo que quanto mais camadas existem, mais complexo é o warehouse.

Em uma organização em três camadas, por exemplo, temos uma camada inicial para a extração dos dados, uma segunda para limpeza e outra para consultas e análises. Assim como podemos ter um Data Warehouse simples, com apenas uma camada.

Vamos então destrinchar componentes que fazem parte de uma arquitetura de DW de tês camadas.

# Bancos de dados
Bancos de dados são coleções organizadas de dados que permitem leitura e escrita, com acesso e recuperação rápidos. Geralmente, surgem em um formato relacional, o que significa que organizam os dados em tabelas (linhas e colunas) que se relacionam logicamente entre si.

Eles fazem parte do conceito de warehouse, sendo um fundamento para esse conceito. Em suma, um DW é um conjunto de bancos de dados com algumas funcionalidades a mais.

# ETL
Em seguida, na arquitetura de um armazém de dados, temos ferramentas ETL. O termo significa “extrair, transformar e carregar”. Trata-se de uma solução que cuida dos dados antes que eles sejam carregados no warehouse.

Primeiro, se extrai os dados de fontes transacionais ou não, como CRM e ERP. Depois, temos a limpeza e a formatação dos dados, com padronização, eliminação de itens faltantes, gestão dos nomes dos arquivos etc. Em seguida, os dados são carregados para o repositório.

Uma solução ETL é essencial para a noção de warehouse, pois é ela que garante a qualidade e o esquema dos dados que entram. Desse modo, é possível utilizar os dados para seus fins analíticos na outra ponta.

# Metadados
Quando falamos em estruturas de armazenamento de dados, precisamos citar a importância dos metadados. Eles descrevem os dados armazenados e auxiliam no trabalho técnico dos desenvolvedores e gestores que dominam essas informações. Os metadados permitem compreender melhor o que está no DW, de modo que esses dados sejam úteis para os fins estabelecidos.

# Data Marts
Outro elemento importante nessas estruturas é o Data Mart. É um conjunto de dados específico para uma análise segmentada e departamental, sendo, portanto, o resultado da divisão dos dados do warehouse em uma camada posterior. Os DMs são pequenos subgrupos de dados que dizem respeito apenas a um determinado setor, de forma a responder perguntas específicas.

Faz pleno sentido a divisão de um repositório centralizado em pequenos subgrupos posteriormente se o objetivo é a análise de dados. Uma vez que esses ativos já estão limpos e formatados, é possível então facilitar as consultas ao oferecer a cada setor os dados necessários rapidamente. Também é fundamental para controle de acesso a dados confidenciais.

# Ferramentas de acesso
Por fim, na arquitetura de um Data Warehouse, temos as ferramentas de acesso. São os sistemas que acessarão os dados dispostos no DW, de modo a efetuar as análises. Pode ser uma solução de Business Intelligence, por exemplo, com o intuito de gerar relatórios completos acerca dos dados, das métricas/indicadores e do histórico de dados. Pode ser também um projeto de Data Science.

As ferramentas de acesso correspondem à visão do usuário final, que busca os dados para visualização, criação de relatórios, mineração dos dados ou treinamento de modelos de machine learning.

Exemplo: </p>
</p>
<img src="https://user-images.githubusercontent.com/91704169/234309355-0c4dbbce-85c6-4629-bfba-847ca6851793.png" width="1000px" align="centter" alt="planos">
