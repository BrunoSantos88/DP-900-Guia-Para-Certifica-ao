# Indentificar serviços de dados

O Microsoft Azure é uma plataforma de nuvem que potencializa os aplicativos e a infraestrutura de TI de algumas das maiores organizações do mundo. Ele inclui muitos serviços para dar suporte a soluções de nuvem, incluindo cargas de trabalho de dados transacionais e analíticas.

Alguns dos serviços de nuvem mais usados para dados estão descritos abaixo.


Este tópico aborda apenas alguns dos serviços de dados mais usados em soluções analíticas e transacionais modernas. Também há serviços adicionais disponíveis.

# SQL do Azure
Azure SQL logoSQL do Azure é o nome coletivo de uma família de soluções de banco de dados relacional com base no mecanismo de banco de dados do Microsoft SQL Server. Os serviços específicos de SQL do Azure incluem:

Banco de Dados SQL do Azure – um banco de dados de PaaS (plataforma como serviço) totalmente gerenciado hospedado no Azure
Instância Gerenciada de SQL do Azure – uma instância hospedada do SQL Server com manutenção automatizada, que permite uma configuração mais flexível do que o BD de SQL do Azure, mas com mais responsabilidade administrativa para o proprietário.
VM de SQL do Azure – uma máquina virtual com uma instalação do SQL Server, permitindo a máxima capacidade de configuração com total responsabilidade de gerenciamento.
Os administradores de banco de dados normalmente provisionam e gerenciam os sistemas de banco de dados SQL do Azure para dar suporte a aplicativos de LOB (linha de negócios) que precisam armazenar dados transacionais.

Os engenheiros de dados podem usar os sistemas de banco de dados SQL do Azure como fontes para pipelines de dados que executam operações de ETL (extração, transformação e carregamento) para ingerir os dados transacionais em um sistema analítico.

Os analistas de dados podem consultar os bancos de dados SQL do Azure diretamente para criar relatórios, no entanto, em grandes organizações, os dados geralmente são combinados com os dados de outras fontes em um armazenamento de dados analíticos para dar suporte às análises empresariais.

# Banco de dados do Azure para bancos dados relacionais de código aberto
Azure Database for MariaDB, MySQL, and PostreSQL logos O Azure inclui serviços gerenciados para sistemas de banco de dados relacionais populares de código aberto, incluindo:

- Banco de Dados do Azure para MySQL – um sistema de gerenciamento de banco de dados de código aberto fácil de usar que é comumente usado em aplicativos da pilha LAMP (Linux, Apache, MySQL e PHP).

- Banco de Dados do Azure para MariaDB – um sistema de gerenciamento de banco de dados mais recente, criado pelos desenvolvedores originais do MySQL. Desde então, o mecanismo de banco de dados foi reescrito e otimizado para aprimorar o desempenho. O MariaDB tem compatibilidade com o Oracle Database (outro sistema de gerenciamento de banco de dados comercial popular).

- Banco de dados do Azure para PostgreSQL – um banco de dados híbrido relacional-objeto. É possível armazenar dados em tabelas relacionais, mas um banco de dados PostgreSQL também permite que você armazene tipos de dados personalizados, com propriedades não relacionais próprias.

Assim como acontece com os sistemas de banco de dados SQL do Azure, os bancos de dados relacionais de código aberto são gerenciados por administradores de banco de dados para dar suporte a aplicativos transacionais e fornecem uma fonte de dados para engenheiros de dados, criando pipelines para soluções analíticas e analistas de dados que criam relatórios.

# Azure Cosmos DB

- Azure Cosmos DB </p>
O Azure Cosmos DB é um sistema de banco de dados não relacional (NoSQL) de escala global que dá suporte a várias APIs (interfaces de programação de aplicativo), permitindo que você armazene e gerencie dados como documentos JSON, pares chave-valor, famílias de colunas e grafos.

Em algumas organizações, instâncias do Cosmos DB podem ser provisionadas e gerenciadas por um administrador de banco de dados, embora os desenvolvedores de software tenham o costume de gerenciar o armazenamento de dados NoSQL como parte da arquitetura geral do aplicativo. Os engenheiros de dados geralmente precisam integrar fontes de dados do Cosmos DB a soluções analíticas corporativas que dão suporte à modelagem e geração de relatórios por analistas de dados.

# Armazenamento do Azure

Azure Storage logo O Armazenamento do Azure é um serviço principal do Azure que permite armazenar dados em:

- Contêineres de blobs – armazenamento escalonável e econômico para arquivos binários.
Compartilhamentos de arquivos – compartilhamentos de arquivos de rede, semelhante ao que normalmente é encontrado nas redes corporativas.
Tabelas – armazenamento de chave-valor para aplicativos que precisam ler e gravar valores de dados rapidamente.
Os engenheiros de dados usam o Armazenamento do Azure para hospedar data lakes – armazenamentos de blobs com um namespace hierárquico que permite que os arquivos sejam organizados em pastas em um sistema de arquivos distribuído.

# Fábrica de dados do Azure (data Factor)
Azure Data Factory logo O Azure Data Factory é um serviço do Azure que permite definir e agendar pipelines de dados para transferir e transformar dados. Você pode integrar seus pipelines a outros serviços do Azure, possibilitando a ingestão de dados de armazenamentos de dados na nuvem, o processamento dos dados usando a computação baseada em nuvem e a manutenção dos resultados em outro armazenamento de dados.

O Azure Data Factory é usado por engenheiros de dados para criar soluções de ETL (extração, transformação e carregamento) que preenchem os armazenamentos de dados analíticos com os dados de sistemas transacionais na organização.

# Azure Synapse Analytics
Azure Synapse Analytics logo O Azure Synapse Analytics é uma solução de análise de dados abrangente e unificada que oferece uma interface de serviço única para vários recursos analíticos, incluindo:

- Pipelines – baseado na mesma tecnologia do Azure Data Factory.
SQL – um mecanismo de banco de dados SQL altamente escalonável, otimizado para cargas de trabalho de data warehouse.
Apache Spark – um sistema de processamento de dados distribuído de código aberto que dá suporte a várias linguagens de programação e APIs, incluindo Java, Scala, Python e SQL.
- Data Explorer do Azure Synapse – uma solução de análise de dados de alto desempenho que é otimizada para consultas em tempo real de dados de log e telemetria usando a KQL (Linguagem de Consulta Kusto).
Os engenheiros de dados podem usar o Azure Synapse Analytics para criar uma solução de análise de dados unificada que combina pipelines de ingestão de dados, armazenamento de data warehouse e armazenamento do data lake em um único serviço.

Os analistas de dados podem usar pools de SQL e do Spark por meio de notebooks interativos para explorar e analisar dados e aproveitar a integração com serviços como Azure Machine Learning e Microsoft Power BI para criar modelos de dados e extrair insights dos dados.

# Azure Databricks
Azure Databricks logo O Azure Databricks é uma versão integrada do Azure da plataforma popular do Databricks, que combina a plataforma de processamento de dados Apache Spark com a semântica de banco de dados SQL e uma interface de gerenciamento integrada para permitir a análise de dados em larga escala.

Os engenheiros de dados podem usar as habilidades que já têm do Databricks e do Spark para criar armazenamentos de dados analíticos no Azure Databricks.

Os analistas de dados podem usar o suporte nativo ao notebook no Azure Databricks para consultar e visualizar dados em uma interface baseada na Web fácil de usar.

# Azure HDInsight
Azure HDInsight logo O Azure HDInsight é um serviço do Azure que fornece clusters hospedados no Azure para tecnologias populares de código aberto de processamento de Big Data do Apache, incluindo:

- Apache Spark – um sistema de processamento de dados distribuído que dá suporte a várias linguagens de programação e APIs, incluindo Java, Scala, Python e SQL.
- Apache Hadoop – um sistema distribuído que usa trabalhos MapReduce para processar grandes volumes de dados com eficiência em vários nós de cluster. Os trabalhos MapReduce podem ser escritos em Java ou abstraídos por interfaces como Apache Hive, uma API baseada em SQL que é executada no Hadoop.
- Apache HBase – um sistema de código aberto para armazenamento e consulta de dados NoSQL em larga escala.
- Apache Kafka – um agente de mensagens para processamento de fluxo de dados.
- Apache Storm – um sistema de código aberto para processamento de dados em tempo real por meio de uma topologia de spouts e bolts.
Os engenheiros de dados podem usar o Azure HDInsight para dar suporte a cargas de trabalho de análise de Big Data que dependem de várias tecnologias de código aberto.

# Stream Analytics do Azure
Azure Stream Analytics logo O Azure Stream Analytics é um mecanismo de processamento de fluxo em tempo real que captura um fluxo de dados de uma entrada, aplica uma consulta para extrair e manipular os dados do fluxo de entrada e grava os resultados em uma saída para análise ou processamento adicional.

Os engenheiros de dados podem incorporar o Azure Stream Analytics em arquiteturas de análise de dados que capturam fluxos dados para ingestão em um armazenamento de dados analíticos ou para visualização em tempo real.

# Azure Data Explorer
Azure Data Explorer logo O Azure Data Explorer é um serviço autônomo que oferece a mesma consulta de alto desempenho de dados de log e telemetria que o runtime do Data Explorer do Azure Synapse no Azure Synapse Analytics.

Os analistas de dados podem usar o Azure Data Explorer para consultar e analisar dados que incluem um atributo de carimbo de data/hora, como normalmente é encontrado em arquivos de log e dados de telemetria da IoT (Internet das Coisas).

# Microsoft Purview
Azure Purview logo O Microsoft Purview fornece uma solução para governança e descoberta de dados de toda a empresa. Use o Microsoft Purview para criar um mapa de seus dados e acompanhar a linhagem de dados em várias fontes de dados e sistemas, permitindo encontrar dados confiáveis para análise e relatórios.

Os engenheiros de dados podem usar o Microsoft Purview para impor a governança de dados em toda a empresa e garantir a integridade dos dados usados para dar suporte a cargas de trabalho analíticas.

# Microsoft Power BI
Microsoft Power BI logo O Microsoft Power BI é uma plataforma para modelagem de dados analíticos e relatórios que os analistas de dados podem usar para criar e compartilhar visualizações de dados interativas. Os relatórios do Power BI podem ser criados por meio do aplicativo Power BI Desktop e, em seguida, publicados e fornecidos por meio de relatórios e aplicativos baseados na Web no serviço do Power BI, bem como no aplicativo móvel do Power BI.
