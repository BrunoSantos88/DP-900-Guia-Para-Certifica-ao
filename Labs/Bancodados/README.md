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

Link: https://azure.microsoft.com/pt-br/products/category/databases

# O que é o Banco de Dados SQL do Azure?

- Aplica-se a: Banco de Dados SQL do Azure

Link: https://learn.microsoft.com/pt-br/azure/azure-sql/database/sql-database-paas-overview?view=azuresql </p>
Link: https://learn.microsoft.com/pt-br/azure/azure-sql/database/doc-changes-updates-release-notes-whats-new?view=azuresql

# Commandos SQL

# DML: consultando e modificando os registros da tabela
O DML, ou Data Manipulation Language é um subconjunto do SQL que diz respeito aos comandos utilizados para manipular diretamente os dados de uma tabela (ou banco de dados).

Com o DML é possível inserir, atualizar, modificar e excluir registros de maneira rápida e direta, sem a necessidade de uma tecnologia intermediária.

Veja, abaixo, os principais comandos.

# Insert: adicionando registros a uma tabela
O insert, como é possível deduzir pela nomenclatura, é o comando que adiciona registros a uma tabela, ou seja, inclui dados em um banco de dados.

Para utilizá-lo, basta escrever a seguinte sintaxe:

- INSERT into [tabela exemplo] (campo1, campo2, campo3) values (dado1, 'dado2', 'dado3');

No exemplo acima, apontamos os campos 1, 2 e 3 na tabela exemplo e, em seguida, descrevemos seus valores (dados 1, 2 e 3).

# Update: atualizando os registros já inseridos
O comando update é utilizado para atualizar registros que já estão inseridos na tabela, mas que por algum motivo precisam ser corrigidos ou complementados.

Para utilizar este comando, basta escrever a seguinte linha:

- UPDATE tabela exemplo SET campo1 = 'dado1' WHERE id = dado2;

No exemplo acima, apontamos que a modificação deve ser feita na tabela exemplo, em seu campo1. Os dados modificados são os dados1 e dado2.

# Delete: excluindo registros de uma tabela
Com o comando delete, podemos excluir registros que estão em uma tabela, eliminando essa informação de toda base de dados. 

Esse comando, no entanto, excluir apenas os registros. Estrutura, índices e outros atributos do projeto continuam sem modificações.

Para utilizá-lo, basta escrever a sintaxe abaixo:

- DELETE FROM tabela exemplo;

No exemplo acima, indicamos que a exclusão deve ser feita na tabela exemplo.

# Select: retomando registros na tabela
O comando select permite que façamos consultas em uma tabela, ou seja, pode ser usado de diversas maneiras diferentes para que diversos tipos de consultas possam ser feitos.

Por exemplo: podemos retomar todos os dados de uma tabela, dados de somente uma coluna, uma única informação em específico, etc.

Para utilizar este comando, há as seguintes opções de código:

- SELECT * FROM tabela exemplo;, onde o * indica que queremos consultar todos os dados da tabela exemplo.
- SELECT dado1, dado2 FROM tabela exemplo;, onde indicamos que queremos consultar somente os dados 1 e 2 da tabela exemplo.
Há, ainda, mais maneiras de utilizar este comando.

 # DDL: criando, alterando e excluindo tabelas de registros
 
Os comandos do subconjunto DDL, ou Data Definition Language, são aqueles utilizados para manipular a estrutura de um banco de dados, e não somente os registros incluídos ali.

Com estes comandos, podemos criar novas tabelas, alterar tabelas já existentes e também exclui-las.

Veja, abaixo, os três principais comandos.

# Create: criando novas tabelas em um banco de 

Com o comando create é possível criar uma nova tabela dentro de um banco de dados.
Para utilizá-lo, é preciso, primeiro, criar um objeto dentro do banco de dados, ou um banco de dados completamente vazio:

- CREATE DATABASE banco exemplo;

No exemplo acima, criamos o banco de dados banco exemplo. Para criar, dentro deste banco, uma tabela, é preciso o comando create table:

- CREATE TABLE tabela exemplo (id INT PRIMARY KEY, campo1 VARCHAR(50), campo2 (VARCHAR(100));

No exemplo acima, criamos a tabela exemplo, onde o comando INT PRIMARY KEY indica que o campo id é a chave primária da tabela, ou seja, a identificação principal do registro. 

Em seguida, estipulamos as colunas com os campos 1 e 2 e, com o comando VARCHAR, definimos a quantidade máxima de caracteres que estes campos comportarão (50 a 100, respectivamente).

# Alter: alterando uma tabela já criada
O comando alter é utilizado para alterar uma tabela pré existente e pode ser manipulado da seguinte maneira:

- ALTER TABLE tabela exemplo ADD nome INT;

No exemplo acima, estamos alterando a tabela exemplo ao adicionar uma nova coluna: a coluna nome.

# Drop: excluindo uma tabela do banco de dados

Enfim, o comando drop é aquele que utilizamos para excluir objetos, ou tabelas, de nossa base de dados.
Esse comando também pode ser utilizados para excluir um banco de dados inteiro, como veremos nos exemplos abaixo.
Com a linha DROP TABLE tabela exemplo;, é possível excluir a tabela exemplo de um banco de dados.
Com a linha DROP DATABASE banco exemplo;, é possível excluir o banco de dados banco exemplo inteiro.

