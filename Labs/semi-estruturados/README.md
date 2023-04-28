# O que é o Armazenamento de Blobs do Azure?

Sobre Armazenamento de Blobs
Sobre o Azure Data Lake Storage Gen2
Próximas etapas
O Armazenamento de Blobs do Azure é uma solução de armazenamento de objetos da Microsoft para a nuvem. O Armazenamento de Blobs é otimizado para armazenar grandes quantidades de dados não estruturados. Dados não estruturados são dados que não estão de acordo com uma definição ou um modelo de dados específico, como texto ou dados binários.

# Sobre Armazenamento de Blobs
O Armazenamento de Blobs foi projetado para:

Fornecimento de imagens ou de documentos diretamente a um navegador.
Armazenamento de arquivos para acesso distribuído.
Transmissão por streaming de áudio e vídeo.
Gravando nos arquivo de log.
Armazenamento de dados de backup e restauração, recuperação de desastres e arquivamento.
Armazenamento de dados para análise por um serviço local ou hospedado no Azure.
Usuários ou aplicativos cliente podem acessar objetos no Armazenamento de Blobs via HTTP/HTTPS de praticamente qualquer lugar no mundo. Objetos no Armazenamento de Blobs estão acessíveis por meio da API REST do Armazenamento do Azure, do Azure PowerShell, da CLI do Azure ou em uma biblioteca de clientes do Armazenamento do Azure. As bibliotecas de cliente estão disponíveis para diferentes idiomas, incluindo:

# Linguagen
.NET
Java
Node.js
Python
Go


Os clientes também podem se conectar com segurança ao Armazenamento de Blobs usando o Protocolo SSH de Transferência de Arquivo (SFTP) e montar contêineres de Armazenamento de Blobs usando o protocolo NFS (Sistema de Arquivos de Rede) 3.0.

Sobre o Azure Data Lake Storage Gen2
O Armazenamento de Blobs dá suporte ao Azure Data Lake Storage Gen2, a solução de análise de Big Data corporativa da Microsoft para a nuvem. O Azure Data Lake Storage Gen2 oferece um sistema de arquivos hierárquico, bem como as vantagens do Armazenamento de Blobs, incluindo:

# Armazenamento em camadas de baixo custo
Alta disponibilidade
Coerência forte
Recursos de recuperação de desastre
Para obter mais informações sobre o Data Lake Storage Gen2, veja a Introdução ao Azure Data Lake Storage Gen2.

O Azure Data Lake Storage Gen2 é um conjunto de funcionalidades dedicadas à análise de Big Data, criado no Armazenamento de Blobs do Azure.

O Data Lake Storage Gen2 converge as funcionalidades do Azure Data Lake Storage Gen1 com o Armazenamento de Blobs do Azure. Por exemplo, o Data Lake Storage Gen2 fornece semântica do sistema de arquivos, segurança em nível de arquivo e escala. Como essas funcionalidades são criadas no Armazenamento de Blobs, você também obtém um armazenamento em camadas de baixo custo, com funcionalidades de alta disponibilidade/recuperação de desastre.

O Data Lake Storage Gen2 torna o armazenamento do Azure a fundação para a criação de data lakes empresariais no Azure. Projetado desde o início para atender a vários petabytes de informações enquanto mantém centenas de gigabits de taxa de transferência, o Data Lake Storage Gen2 permite que você gerencie de uma maneira fácil grandes quantidades de dados.

# O que é um Data Lake?

Um data lake é um repositório único e centralizado onde você pode armazenar todos os seus dados, estruturados e não estruturados. Um data lake permite que sua organização armazene, acesse e analise com mais facilidade e rapidez uma ampla variedade de dados em um único local. Com um data lake, você não precisa conformar os seus dados para que se ajustem a uma estrutura existente. Em vez disso, você pode armazenar seus dados no formato bruto ou nativo, geralmente como arquivos ou como objetos binários grandes (blobs).

O Azure Data Lake Storage é uma solução de data lake corporativa baseada em nuvem. Ele foi projetado para armazenar grandes quantidades de dados em qualquer formato e facilitar cargas de trabalho analíticas de Big Data. Pode ser usado para capturar dados de qualquer tipo e velocidade de ingestão em um único local e assim facilitar o seu acesso e análise usando várias estruturas.

Data Lake Storage Gen2
O Azure Data Lake Storage Gen2 refere-se à implementação atual da solução do Data Lake Storage do Azure. A implementação anterior, Azure Data Lake Storage Gen1, será desativada em 29 de fevereiro de 2024.

Ao contrário do Data Lake Storage Gen1, o Data Lake Storage Gen2 não é um serviço ou tipo de conta dedicado. Em vez disso, ele é implementado como um conjunto de recursos que você utiliza com o serviço de Armazenamento de Blobs da sua conta de Armazenamento do Microsoft Azure. Você pode desbloquear esses recursos habilitando a configuração do namespace hierárquico.

O Data Lake Storage Gen2 inclui as seguintes funcionalidades.

✓ Acesso compatível com Hadoop

✓ Estrutura hierárquica de diretórios

✓ Custo e desempenho otimizados

✓ Modelo de segurança de granularidade mais refinado

✓ Escalabilidade em massa

Acesso compatível com Hadoop
O Azure Data Lake Storage Gen2 foi projetado principalmente para funcionar com o Hadoop e todas as estruturas que utilizam o Apache Sistema de Arquivos Distribuído Hadoop (HDFS) como sua camada de acesso a dados. As distribuições do Hadoop incluem o driver do Azure Blob File System (ABFS), que permite que muitos aplicativos e estruturas acessem diretamente os dados do Armazenamento de Blobs do Azure. O driver ABFS é otimizado especificamente para análise de Big Data. As APIs REST correspondentes são exibidas pelo ponto de extremidade, dfs.core.windows.net.

As estruturas de análise de dados que utilizam o HDFS como sua camada de acesso a dados podem acessar diretamente os dados do Azure Data Lake Storage Gen2 através do ABFS. O mecanismo de análise do Apache Spark e o mecanismo de consulta do Presto SQL são exemplos de tais estruturas.

Para obter mais informações sobre os serviços e plataformas compatíveis, confira Serviços do Azure com suporte ao Azure Data Lake Storage Gen2 e Plataformas de código aberto com suporte ao Azure Data Lake Storage Gen2.

Estrutura hierárquica de diretórios
O namespace hierárquico é um recurso importante que permite que o Azure Data Lake Storage Gen2 forneça acesso a dados de alto desempenho em escala e preço de armazenamento de objetos. Você pode usar esse recurso para organizar todos os objetos e arquivos na sua conta de armazenamento em uma hierarquia de diretórios e subdiretórios aninhados. Em outras palavras, seus dados do Azure Data Lake Storage Gen2 são organizados da mesma forma que os arquivos são organizados no seu computador.

Operações como renomear ou excluir um diretório se tornam operações de metadados atômicas únicas no diretório. Não é necessário enumerar e processar todos os objetos que compartilham o prefixo de nome do diretório.

Custo e desempenho otimizados
O preço do Azure Data Lake Storage Gen2 é baseado nos níveis do Armazenamento de Blobs do Azure. Ele se baseia nos recursos de Armazenamento de Blobs do Azure, como o gerenciamento automatizado de políticas de ciclo de vida e as camadas no nível do objeto, para gerenciar os custos da armazenamento de Big Data.

O desempenho é otimizado porque você não precisa copiar ou transformar dados como um pré-requisito para análise. O recurso de namespace hierárquico do Azure Data Lake Storage permite acesso e navegação eficientes. Essa arquitetura significa que o processamento de dados requer menos recursos computacionais, reduzindo o tempo e o custo de acesso aos dados.

Modelo de segurança de granularidade mais refinado
O modelo de controle de acesso do Azure Data Lake Storage Gen2 suporta o controle de acesso baseado em funções do Azure (Azure RBAC) e às listas de controle de acesso (ACLs) da Interface de Sistema Operacional Portátil para UNIX (POSIX). Há também algumas configurações de segurança extras específicas para o Azure Data Lake Storage Gen2. Você pode definir permissões no nível do diretório ou no nível do arquivo. Todos os dados armazenados são criptografados em repouso usando chaves de criptografia gerenciadas pela Microsoft ou pelo cliente.

Escalabilidade em massa
O Azure Data Lake Storage Gen2 oferece armazenamento em massa e aceita vários tipos de dados para análise. Ele não impõe qualquer limite de tamanho de conta, tamanho de arquivo ou volume de dados que podem ser armazenados em um data lake. Arquivos individuais podem ter tamanhos que variam de alguns kilobytes (KBs) a alguns petabytes (PBs). O processamento é executado em latências por solicitação quase constantes que são medidas nos níveis de serviço, conta e arquivo.

Esse design significa que o Azure Data Lake Storage Gen2 pode ser dimensionado com facilidade e rapidez para atender às cargas de trabalho mais exigentes. Ele também pode reduzir verticalmente com facilidade quando a demanda diminuir.

Baseado no Armazenamento de Blobs do Azure
Os dados que você ingere persistem como blobs na conta de armazenamento. O serviço que gerencia os blobs é o serviço Armazenamento de Blobs do Azure. O Data Lake Storage Gen2 descreve os recursos ou "aprimoramentos" desse serviço que atendem às demandas de cargas de trabalho analíticas de Big Data.

Como esses recursos são baseados no Armazenamento de Blobs, recursos como log de diagnóstico, camadas de acesso e políticas de gerenciamento do ciclo de vida estão disponíveis na sua conta. A maioria dos recursos do Armazenamento de Blobs são totalmente suportados, mas alguns recursos podem ser suportados apenas em nível de pré-visualização e há alguns deles que ainda não são suportados. Para obter uma lista completa das instruções de suporte, confira Suporte ao recurso de Armazenamento de Blobs nas contas de Armazenamento do Microsoft Azure. O status de cada recurso listado será alterado com o tempo, à medida que o suporte continuar a se expandir.

Documentação e terminologia
O sumário do Armazenamento de Blobs do Azure apresenta duas seções de conteúdo. A seção de conteúdo Data Lake Storage Gen2 fornece as melhores práticas e diretrizes para o uso dos recursos do Data Lake Storage Gen2. A seção de conteúdos do Armazenamento de Blobs fornece diretrizes para recursos da conta não específicos do Data Lake Storage Gen2.

À medida que você se move entre as seções, você pode notar algumas pequenas diferenças de terminologia. Por exemplo, o conteúdo em destaque na documentação do Armazenamento de Blobs usará o termo blob em vez de arquivo. Tecnicamente, os arquivos ingeridos na sua conta de armazenamento se tornam blobs em sua conta. Portanto, o termo está correto. No entanto, o termo blob poderá causar confusão se você estiver habituado com o termo arquivo. Você também verá o termo contêiner usado para se referir a um sistema de arquivos. Considere esses termos como sinônimos.
