# Explorar bancos de dados

Um banco de dados é usado para definir um sistema central no qual dados podem ser armazenados e consultados. De maneira simplista, o sistema de arquivos no qual os arquivos são armazenados é um tipo de banco de dados; mas quando usamos o termo em um contexto de dados profissional, normalmente nos referimos a um sistema dedicado para gerenciar registros de dados em vez de arquivos.

Bancos de dados relacionais
Os bancos de dados relacionais são comumente usados para armazenar e consultar dados estruturados. Os dados são armazenados em tabelas que representam entidades, como clientes, produtos ou pedidos de venda. Cada instância de uma entidade recebe uma chave primária que a identifica de maneira exclusiva. Essas chaves são usadas para fazer referência à instância da entidade em outras tabelas. Por exemplo, a chave primária de um cliente pode ser referenciada em um registro de pedido de venda para indicar qual cliente fez o pedido. Esse uso de chaves para referenciar entidades de dados permite que um banco de dados relacional seja normalizado, o que, em parte, significa a eliminação de valores de dados duplicados para que, por exemplo, os detalhes de um cliente individual sejam armazenados apenas uma vez e não para cada pedido de vendas que o cliente faz. As tabelas são gerenciadas e consultadas usando SQL (linguagem SQL), que se baseia em um padrão ANSII e que, portanto, é semelhante entre vários sistemas de banco de dados.

# Bancos de dados não relacionais

Os bancos de dados não relacionais são sistemas de gerenciamento de dados que não aplicam um esquema relacional aos dados. Os bancos de dados não relacionais geralmente são chamados de banco de dados NoSQL, embora alguns ofereçam suporte a uma variante da linguagem SQL.

Há quatro tipos comuns de banco de dados não relacionais normalmente em uso.

Bancos de dados de chave-valor nos quais cada registro consiste em uma chave exclusiva e um valor associado, que pode estar em qualquer formato.

Bancos de dados de documentos, que são uma forma específica de banco de dados de chave-valor na qual o valor é um documento JSON (em que o sistema é otimizado para análise e consulta)

Bancos de dados de família de colunas que podem armazenar dados tabulares que abrangem linhas e colunas; você também pode dividir as colunas em grupos conhecidos como famílias de colunas. Cada família de colunas contém um conjunto de colunas que estão logicamente relacionadas.

Bancos de dados de grafo, que armazenam entidades como nós com links para definir relações entre eles.

# Tipos de Bancos de Dados no Azure
Serviços de banco de dados em nuvem totalmente gerenciados, inteligentes e flexíveis

O Azure oferece uma opção de bancos de dados relacionais, NoSQL e em memória totalmente gerenciados. Eles abrangem mecanismos proprietários e de código aberto a fim de atender às necessidades dos desenvolvedores de aplicativos modernos. O gerenciamento de infraestrutura, incluindo escalabilidade, disponibilidade e segurança, é automatizado, economizando tempo e dinheiro. Concentre-se na criação de aplicativos enquanto os bancos de dados gerenciados do Azure simplificam seu trabalho com insights de desempenho via inteligência incorporada, dimensionamento ilimitado e gerenciamento contra ameaças à segurança.

Localize o produto de banco de dados que atenda a suas necessidades Se desejar	Use isto.

- Crie aplicativos que são escalados com o banco de dados SQL inteligente e gerenciado na nuvem	Banco de Dados SQL do Azure
Modernize os aplicativos do SQL Server com uma instância SQL gerenciada e sempre atualizada na nuvem	Instância Gerenciada de SQL do Azure
Migre suas cargas de trabalho do SQL para o Azure mantendo a compatibilidade do SQL Server e o acesso em nível de sistema operacional completos	SQL Server em Máquinas Virtuais do Azure

- Crie aplicativos para empresas totalmente gerenciados, seguros e escalonáveis no PostgreSQL de código aberto, escale horizontalmente o PostgreSQL de nó único com alto desempenho ou migre cargas de trabalho do PostgreSQL e do Oracle para a nuvem	Banco de Dados do Azure para PostgreSQL

- Forneça alta disponibilidade e dimensionamento elástico a aplicativos móveis e Web de código aberto com um serviço de banco de dados MySQL da comunidade gerenciado ou migre cargas de trabalho MySQL para a nuvem	Banco de Dados do Azure para MySQL

- Forneça alta disponibilidade e dimensionamento elástico a aplicativos móveis e Web de código aberto com um serviço de banco de dados MariaDB da comunidade gerenciado	Banco de Dados do Azure para MariaDB

- Crie aplicativos com garantia de baixa latência e de alta disponibilidade em qualquer lugar, em qualquer escala, ou migre o Cassandra, o MongoDB e outras cargas de trabalho NoSQL para a nuvem	Azure Cosmos DB

- Forneça aplicativos rápidos e escalonáveis com um armazenamento de dados em memória compatível com código aberto	Cache do Azure para Redis.

- Acelere sua transição para a nuvem usando um processo de migração simples e autodirigido	Serviço de Migração de Banco de Dados do Azure

- Modernize os aplicativos e clusters de dados do Cassandra e desfrute de flexibilidade e liberdade com o serviço de instância gerenciada	Instância Gerenciada do Azure para Apache Cassandra
