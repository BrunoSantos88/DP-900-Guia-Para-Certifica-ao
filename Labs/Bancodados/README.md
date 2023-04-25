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
