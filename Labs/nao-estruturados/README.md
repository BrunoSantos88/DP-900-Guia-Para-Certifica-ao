# Não estruturados

Ao contrário dos dados estruturados, os dados não estruturados possuem uma estrutura totalmente inversa e não podem ser organizados em tabelas.

Esse tipo de dados não tem uma estrutura bem definida, não tem um padrão pré-estabelecido. São dados flexíveis e dinâmicos, podendo ser compostos por diversos elementos diferentes dentro um todo.

Um exemplo simples de dados não estruturados são os dados de redes sociais. Esse é um típico exemplo, pelo grande número de textos, imagens, vídeos e diversos outros que são criados diariamente a partir do uso das tecnologias.

Na verdade, a maior parte dos dados gerados no mundo todo são dados não estruturados, tendo aproximadamente o percentual de 80%. Esses dados têm uma complexidade um pouco maior para análise, já que são informações de difícil processamento e recuperação, pois não contam com componentes necessários para a sua identificação. Porém, com a disponibilização de tecnologias que nos ajudam nesse quesito, essa complexidade da análise de dados tem diminuído.


# Dados não relacionais e NoSQL

Um banco de dados não relacional é um banco de dados que não usa o esquema de tabela de linhas e colunas encontrado na maioria dos sistemas de banco de dados tradicionais. Em vez disso, os bancos de dados não relacionais usam um modelo de armazenamento otimizado para os requisitos específicos do tipo de dados que está sendo armazenado. Por exemplo, os dados podem ser armazenados como pares chave/valor simples, como documentos JSON ou como um gráfico que consiste em bordas e vértices.

O que esses armazenamentos de dados têm em comum é que eles não usam um modelo relacional. Além disso, eles tendem a ser mais específicos no tipo de dados ao qual dão suporte e no modo como os dados podem ser consultados. Por exemplo, os armazenamentos de dados de série temporal são otimizados para consultas em sequências de dados baseadas em tempo. No entanto, os armazenamentos de dados de grafo são otimizados para explorar as relações ponderadas entre entidades. Nenhum dos dois formatos será bem generalizado para a tarefa de gerenciamento de dados transacionais.

O termo NoSQL refere-se aos armazenamentos de dados que não usam o SQL para consultas. Em vez disso, os armazenamentos de dados usam outras linguagens de programação e constructos para consultar os dados. Na prática, "NoSQL" significa "banco de dados não relacionais", mesmo que muitos desses bancos de dados deem suporte a consultas compatíveis com SQL. No entanto, a estratégia de execução de consulta subjacente é geralmente muito diferente da maneira como um RDBMS tradicional executa a mesma consulta SQL.

As seções a seguir descrevem as principais categorias de banco de dados não relacional ou NoSQL.

# Armazenamentos de dados de documentos

Um armazenamento de dados de documento gerencia um conjunto de campos de cadeia de caracteres nomeados e valores de dados de objeto em uma entidade conhecida como documento. Normalmente, esses repositórios de dados armazenam dados na forma de documentos JSON. Cada valor de campo pode ser um item escalar, como um número ou um elemento composto, como uma lista ou uma coleção de pai-filho. Os dados nos campos de um documento podem ser codificados de várias maneiras, incluindo XML, YAML, JSON, BSON ou, até mesmo, armazenados como texto sem formatação. Os campos nos documentos são expostos ao sistema de gerenciamento de armazenamento, permitindo que um aplicativo consulte e filtre dados utilizando os valores nesses campos.

Normalmente, um documento contém todos os dados de uma entidade. Quais itens constituem uma entidade são específicos do aplicativo. Por exemplo, uma entidade pode conter os detalhes de um cliente, um pedido ou uma combinação de ambos. Um único documento pode conter informações que serão distribuídas em várias tabelas relacionais em um RDBMS. Um repositório de documentos não requer que todos os documentos tenham a mesma estrutura. Essa abordagem em forma livre oferece grande flexibilidade. Por exemplo, os aplicativos podem armazenar dados diferentes em documentos, em resposta a uma alteração nos requisitos de negócios.


O aplicativo pode recuperar documentos utilizando a chave de documento. A chave é um identificador exclusivo do documento, que geralmente tem um hash, para ajudar a distribuir os dados de maneira uniforme. Alguns bancos de dados de documentos criam a chave do documento automaticamente. Outros permitem que você especifique um atributo do documento a ser usado como chave. O aplicativo também pode consultar documentos com base no valor de um ou mais campos. Alguns bancos de dados de documentos dão suporte à indexação para facilitar a pesquisa rápida de documentos com base em um ou mais campos indexados.

Muitos bancos de dados de documentos fornecem suporte a atualizações in loco, permitindo que um aplicativo modifique os valores de campos específicos em um documento sem regravar o documento inteiro. As operações de leitura e gravação em vários campos em um só documento normalmente são atômicas.

Serviço do Azure relevante:
- Azure Cosmos DB

# Armazenamentos de dados de colunas
Um armazenamento de dados de colunas ou de família de colunas organiza os dados em colunas e linhas. Em sua forma mais simples, um armazenamento de dados de família de colunas pode parecer muito semelhante a um banco de dados relacional, pelo menos conceitualmente. O poder real de um banco de dados de família de colunas está em sua abordagem desnormalizada para a estruturação de dados esparsos, que deriva da abordagem orientada por coluna para armazenar dados.

- É possível pensar em um armazenamento de dados de família de colunas como contendo dados de tabela com linhas e colunas, mas as colunas são divididas em grupos conhecidos como famílias de colunas. Cada família de colunas contém um conjunto de colunas que estão logicamente relacionadas e geralmente são recuperadas ou manipuladas como uma unidade. Outros dados acessados separadamente podem ser armazenados em famílias de colunas separadas. Dentro de uma família de colunas, novas colunas podem ser adicionadas dinamicamente e as linhas podem ser esparsas (ou seja, uma linha não precisa ter um valor para cada coluna).

- O diagrama a seguir mostra um exemplo com duas famílias de colunas, Identity e Contact Info. Os dados de uma única entidade têm a mesma chave de linha em cada família de colunas. Essa estrutura, em que as linhas de determinado objeto em uma família de colunas podem variar dinamicamente, é um benefício importante da abordagem de família de colunas, que torna essa forma de armazenamento de dados altamente adequada para armazenar dados com esquemas variados.

Ao contrário de um repositório de valor/chave ou um banco de dados de documentos, a maioria dos bancos de dados de família de colunas armazenam dados fisicamente em ordem de chave, em vez de computar um hash. A chave de linha é considerada o índice primário e permite o acesso baseado em chave por meio de uma chave específica ou um intervalo de chaves. Algumas implementações permitem que você crie índices secundários em colunas específicas de uma família de colunas. Os índices secundários permitem recuperar dados por valor de colunas, em vez da chave de linha.

No disco, todas as colunas de uma família de colunas são armazenadas juntas no mesmo arquivo, com um número específico de linhas em cada arquivo. Com conjuntos de dados grandes, esse método cria um benefício de desempenho, reduzindo a quantidade de dados que precisam ser lidos do disco quando apenas algumas colunas são consultadas juntas por vez.

As operações de leitura e gravação para uma linha normalmente são atômicas em uma só família de colunas, embora algumas implementações forneçam atomicidade em toda a linha, abrangendo várias famílias de colunas.

#  Serviço do Azure relevante:

- Azure Cosmos DB for Apache Cassandra
- HBase no HDInsight
