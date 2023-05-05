# O que é processamento em lote?
O processamento em lote é quando um computador processa várias tarefas reunidas em um grupo. Ele foi projetado para ser um processo totalmente automatizado, sem intervenção humana. Também pode ser chamado de automação de carga de trabalho (WLA) e agendamento de tarefas.

O processamento em lote é uma maneira incrivelmente econômica de processar grandes quantidades de dados em um curto período de tempo. Uma vez iniciado o processo, o computador só para quando descobre um erro ou anormalidade, notificando o funcionário ou gerente apropriado.


# Quando utilizar esta solução

O processamento em lotes é utilizado em vários cenários, desde transformações de dados simples a um pipeline ETL (extração-transformação-carga) mais completo. Num contexto de macrodados, o processamento em lotes pode funcionar em conjuntos de dados muito grandes, onde a computação demora muito tempo. (Por exemplo, veja Arquitetura lambda.) Normalmente, o processamento em lotes leva a uma exploração interativa adicional, fornece os dados preparados para modelação para machine learning ou escreve os dados num arquivo de dados otimizado para análise e visualização.

Um exemplo de processamento em lotes é transformar um grande conjunto de ficheiros CSV ou JSON planos e semiestruturados num formato estruturado e esquematizado que está pronto para consulta adicional. Normalmente, os dados são convertidos a partir dos formatos não processados utilizados para ingestão (como CSV) em formatos binários que são mais eficazes para consulta porque armazenam dados num formato columnar e, muitas vezes, fornecem índices e estatísticas inline sobre os dados.

# Desafios
Formatação e codificação de dados. Alguns dos problemas mais difíceis de depurar ocorrem quando os ficheiros utilizam um formato ou codificação inesperados. Por exemplo, os ficheiros de origem podem utilizar uma mistura de codificação UTF-16 e UTF-8 ou conter delimitadores inesperados (espaço versus separador) ou incluir carateres inesperados. Outro exemplo comum são os campos de texto que contêm separadores, espaços ou vírgulas que são interpretados como delimitadores. A lógica de carregamento e análise de dados tem de ser suficientemente flexível para detetar e lidar com estes problemas.

Orquestrar setores de tempo. Muitas vezes, os dados de origem são colocados numa hierarquia de pastas que reflete o processamento de janelas, organizadas por ano, mês, dia, hora, etc. Em alguns casos, os dados podem chegar atrasados. Por exemplo, suponha que um servidor Web falha e os registos de 7 de março só acabam na pasta de processamento a 9 de março. São ignorados porque são demasiado tarde? A lógica de processamento a jusante pode processar registos fora de ordem?

# Arquitetura
Uma arquitetura de processamento em lote tem os seguintes componentes lógicos, apresentados no diagrama acima.

Armazenamento de dados. Normalmente, um arquivo de ficheiros distribuído que pode servir de repositório para grandes volumes de ficheiros grandes em vários formatos. Genericamente, este tipo de arquivo é frequentemente referido como um data lake.

Processamento em lotes. A natureza de grande volume dos macrodados geralmente significa que as soluções têm de processar ficheiros de dados através de tarefas de lote de execução prolongada para filtrar, agregar e, de outra forma, preparar os dados para análise. Normalmente, estes trabalhos envolvem ler os ficheiros de origem, processá-los e escrever a saída em ficheiros novos.

Arquivo de dados analíticos. Muitas soluções de macrodados foram concebidas para preparar dados para análise e, em seguida, servir os dados processados num formato estruturado que pode ser consultado com ferramentas analíticas.

Análises e relatórios. O objetivo da maioria das soluções de macrodados é proporcionar informações sobre os dados através de análises e relatórios.

Orquestração. Com o processamento em lotes, normalmente é necessária alguma orquestração para migrar ou copiar os dados para o seu armazenamento de dados, processamento em lote, arquivo de dados analíticos e camadas de relatórios.

# Opções de tecnologia
As seguintes tecnologias são opções recomendadas para soluções de processamento em lotes no Azure.

# Armazenamento de dados

Contentores de Blobs de Armazenamento do Azure. Muitos processos empresariais existentes do Azure já utilizam o armazenamento de blobs do Azure, o que torna esta uma boa opção para um arquivo de macrodados.
Azure Data Lake Store. O Azure Data Lake Store oferece armazenamento praticamente ilimitado para qualquer tamanho de ficheiro e opções de segurança extensas, tornando-a uma boa opção para soluções de macrodados de grande escala que requerem um arquivo centralizado para dados em formatos heterogéneos.
Para obter mais informações, veja Armazenamento de dados.

# Processamento em lotes
U-SQL. O U-SQL é a linguagem de processamento de consultas utilizada pelo Azure Data Lake Analytics. Combina a natureza declarativa do SQL com a extensibilidade processual de C#e tira partido do paralelismo para permitir um processamento eficiente de dados em grande escala.
Hive. O Hive é um idioma semelhante ao SQL que é suportado na maioria das distribuições do Hadoop, incluindo o HDInsight. Pode ser utilizado para processar dados de qualquer arquivo compatível com HDFS, incluindo o armazenamento de blobs do Azure e o Azure Data Lake Store.
Porco. Pig é uma linguagem declarativa de processamento de macrodados utilizada em muitas distribuições do Hadoop, incluindo o HDInsight. É particularmente útil para o processamento de dados não estruturados ou semiestruturados.
Spark. O motor do Spark suporta programas de processamento em lotes escritos numa série de idiomas, incluindo Java, Scala e Python. O Spark utiliza uma arquitetura distribuída para processar dados em paralelo em vários nós de trabalho.
Para obter mais informações, veja Processamento do Batch.

# Arquivo de dados analítico
Azure Synapse Analytics. Azure Synapse é um serviço gerido baseado em tecnologias de base de dados SQL Server e otimizado para suportar cargas de trabalho de armazenamento de dados em larga escala.
SPARK SQL. O SPARK SQL é uma API criada no Spark que suporta a criação de dataframes e tabelas que podem ser consultadas com a sintaxe SQL.
HBase. O HBase é um arquivo NoSQL de baixa latência que oferece uma opção flexível e de elevado desempenho para consultar dados estruturados e semiestruturados.
Hive. Além de ser útil para o processamento em lotes, o Hive oferece uma arquitetura de base de dados que é conceptualmente semelhante à de um sistema típico de gestão de bases de dados relacionais. Melhorias no desempenho de consultas do Hive através de inovações como o motor Tez e a iniciativa Stinger significam que as tabelas do Hive podem ser utilizadas eficazmente como origens para consultas analíticas em alguns cenários.
Para obter mais informações, veja Arquivos de dados analíticos.

# Análises e relatórios
Azure Analysis Services. Muitas soluções de macrodados emulam arquiteturas de business intelligence empresariais tradicionais ao incluir um modelo de dados centralizado de processamento analítico online (OLAP) (muitas vezes referido como um cubo) no qual os relatórios, dashboards e análise interativa de "segmentação e dados" podem ser baseados. Azure Analysis Services suporta a criação de modelos tabulares para satisfazer esta necessidade.
Power BI. O Power BI permite que os analistas de dados criem visualizações de dados interativas com base em modelos de dados num modelo OLAP ou diretamente a partir de um arquivo de dados analítico.
Microsoft Excel. Microsoft Excel é uma das aplicações de software mais utilizadas no mundo e oferece uma grande variedade de capacidades de análise e visualização de dados. Os analistas de dados podem utilizar o Excel para criar modelos de dados de documentos a partir de arquivos de dados analíticos ou para obter dados de modelos de dados OLAP em tabelas dinâmicas e gráficos interativos.
Para obter mais informações, veja Análise e relatórios.

# Orquestração
Azure Data Factory. Azure Data Factory pipelines podem ser utilizados para definir uma sequência de atividades, agendadas para janelas temporais periódicas. Estas atividades podem iniciar operações de cópia de dados, bem como tarefas do Hive, Pig, MapReduce ou Spark em clusters do HDInsight a pedido; Tarefas U-SQL no Azure Date Lake Analytics; e procedimentos armazenados na Base de Dados Azure Synapse ou SQL do Azure.
Oozie e Sqoop. O Oozie é um motor de automatização de tarefas para o ecossistema do Apache Hadoop e pode ser utilizado para iniciar operações de cópia de dados, bem como tarefas do Hive, Pig e MapReduce para processar dados e tarefas do Sqoop para copiar dados entre bases de dados HDFS e SQL.
Para obter mais informações, veja Orquestração de pipelines

Link: https://learn.microsoft.com/pt-pt/azure/architecture/data-guide/big-data/batch-processing
