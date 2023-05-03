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
