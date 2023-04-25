# Arquiteturas de data warehouse
As seguintes arquiteturas de referência mostram arquiteturas de data warehouse de ponta a ponta no Azure:

BI empresarial no Azure com o Azure Synapse Analytics. Essa arquitetura de referência implementa um pipeline de ELT (extração, carregamento e transformação) que move dados de um banco de dados SQL Server local para o Azure Synapse.
BI empresarial automatizado com o Azure Synapse e o Azure Data Factory. Essa arquitetura de referência mostra um pipeline de ELT com carregamento incremental, automatizado usando o Azure Data Factory.
Quando usar esta solução
Escolha um data warehouse quando precisar transformar grandes quantidades de dados de sistemas operacionais em um formato fácil de entender. Os data warehouses não precisam seguir a mesma estrutura de dados concisa que você pode estar usando em seus bancos de dados OLTP. Você pode usar nomes de coluna que fazem sentido para usuários e analistas de negócios, reestruturar o esquema para simplificar relações e consolidar várias tabelas em uma. Essas etapas ajudam a orientar os usuários que precisam criar relatórios e analisar os dados em sistemas de BI, sem a ajuda de DBAs (Administradores de Banco de Dados) ou de desenvolvedores de dados.

Considere o uso de um data warehouse quando precisar manter dados históricos separados de sistemas de transação de origem por motivos de desempenho. Os data warehouses facilitam o acesso a dados históricos de vários locais, fornecendo uma localização centralizada usando formatos, chaves e modelos de dados comuns.

Como os data warehouses são otimizados para acesso de leitura, a geração de relatórios é mais rápida do que usar o sistema de transações de origem para relatórios.

# Outros benefícios incluem:

O data warehouse pode armazenar dados históricos de várias fontes, representando uma fonte de verdade única.
Você pode aprimorar a qualidade dos dados limpando-os conforme são importados para o data warehouse.
As ferramentas de relatório não competem com os sistemas transacionais em relação aos ciclos de processamento de consulta. Para permitir que o sistema transacional se concentre no tratamento de gravações, um data warehouse atende à maioria das solicitações de leitura.
Um data warehouse pode consolidar dados de programas de software diferentes.
As ferramentas de mineração de dados podem encontrar padrões ocultos nos dados usando metodologias automáticas.
Os data warehouses facilitam o fornecimento de acesso seguro aos usuários autorizados, enquanto restringem o acesso a outras pessoas. Os usuários empresariais não precisam de acesso aos dados de origem, o que elimina um possível vetor de ataque.
Os data warehouses facilitam a criação de soluções de business intelligence, como cubos OLAP.
Desafios
A configuração correta de um data warehouse para atender às necessidades de sua empresa pode trazem alguns dos seguintes desafios:

Confirmar o tempo necessário para modelar corretamente os conceitos de negócios. Os data warehouses são orientados por informações. Você deve padronizar termos relacionados a negócios e formatos comuns, como moeda e datas. Você também precisa reestruturar o esquema de uma forma que faça sentido para os usuários empresariais, mas que ainda garanta a precisão das agregações e relações de dados.

Planejar e configurar a orquestração de dados. Considere como copiar dados do sistema transacional de origem para o data warehouse e quando mover dados históricos de armazenamentos de dados operacionais para o warehouse.

# Manter ou melhorar a qualidade de dados, limpando os dados conforme eles são importados para o warehouse.

# Armazém de dados no Azure

Você pode ter uma ou mais fontes de dados, seja de transações de clientes, seja de aplicativos de negócios. Tradicionalmente, esses dados são armazenados em um ou mais bancos de dados OLTP. Os dados podem ser persistidos em outros meios de armazenamento, como compartilhamentos de rede, Azure Storage Blobs ou um data lake. Os dados também podem ser armazenados pelo próprio data warehouse ou em um banco de dados relacional, como o Banco de Dados SQL do Azure. A finalidade da camada de armazenamento de dados analíticos é atender às consultas emitidas pelas ferramentas de análise e relatório no data warehouse. No Azure, essa funcionalidade de armazenamento analítico pode ser atendida com o Azure Synapse ou com o Azure HDInsight usando o Hive ou o Interactive Query. Além disso, você precisará de algum nível de orquestração para mover ou copiar dados do armazenamento para o data warehouse, o que pode ser feito com o Azure Data Factory ou o Oozie no Azure HDInsight.

Há várias opções para a implementação de um data warehouse no Azure, dependendo de suas necessidades. As listas a seguir são divididas em duas categorias, SMP (multiprocessamento simétrico) e MPP (processamento paralelo em massa).
