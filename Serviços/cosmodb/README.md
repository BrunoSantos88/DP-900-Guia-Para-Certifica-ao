# Azure Cosmos DB

- Azure Cosmos DB </p>

O Azure Cosmos DB é um sistema de banco de dados não relacional (NoSQL) de escala global que dá suporte a várias APIs (interfaces de programação de aplicativo), permitindo que você armazene e gerencie dados como documentos JSON, pares chave-valor, famílias de colunas e grafos.

Em algumas organizações, instâncias do Cosmos DB podem ser provisionadas e gerenciadas por um administrador de banco de dados, embora os desenvolvedores de software tenham o costume de gerenciar o armazenamento de dados NoSQL como parte da arquitetura geral do aplicativo. Os engenheiros de dados geralmente precisam integrar fontes de dados do Cosmos DB a soluções analíticas corporativas que dão suporte à modelagem e geração de relatórios por analistas de dados.


# O que é o Azure Cosmos DB for Apache Gremlin?

Benefícios da API para Gremlin

APLICA-SE A:  Gremlin

- O Azure Cosmos DB é um banco de dados relacional e NoSQL totalmente gerenciado para o desenvolvimento de aplicativos modernos.

- O Azure Cosmos DB for Apache Gremlin é um serviço de banco de dados de grafo que pode ser usado para armazenar grafos grandes com bilhões de vértices e bordas. Você pode consultar os grafos com latência de milissegundo e desenvolver a estrutura do grafo facilmente. A API para Gremlin é criada com base no Apache TinkerPop, uma estrutura de computação de grafo que usa a linguagem de consulta Gremlin.

- Benefícios da API para Gremlin
A API para Gremlin adicionou os benefícios de ser criada no Azure Cosmos DB:

- Taxa de transferência e armazenamento escalonáveis elasticamente: grafos no mundo real precisam ser dimensionados além da capacidade de um único servidor. O Azure Cosmos DB oferece suporte a bancos de dados de grafo escalonáveis horizontalmente que podem ter um tamanho ilimitado em termos de armazenamento e taxa de transferência provisionada. À medida que aumenta a escala do banco de dados do grafo, os dados serão distribuídos automaticamente usando o particionamento do grafo.

- Replicação em várias regiões: o Azure Cosmos DB pode replicar automaticamente seus dados de grafo para qualquer região do Azure no mundo. A replicação global simplifica o desenvolvimento de aplicativos que exigem acesso global aos dados. Além de minimizar a latência de leitura e gravação em qualquer lugar do mundo, o Azure Cosmos DB fornece um mecanismo de failover regional gerenciado por serviço. Esse mecanismo pode garantir a continuidade do aplicativo no caso raro de interrupção de serviço em uma região.

- Consultas e travessias rápidas com o padrão de consulta de grafo mais adotado: armazene vértices e bordas heterogêneos e consulte-os por meio de uma sintaxe conhecida do Gremlin. O Gremlin é uma linguagem de consulta imperativa e funcional que fornece uma interface avançada para implementar algoritmos de grafo comuns. A API para Gremlin habilita travessias e consultas avançadas em tempo real sem a necessidade de especificar dicas de esquema, índices secundários ou exibições. Para obter mais informações, veja consultar grafos usando o Gremlin.

- Banco de dados de grafo totalmente gerenciado: o Azure Cosmos DB elimina a necessidade de gerenciar recursos do computador e do banco de dados. A maioria das plataformas existentes de banco de dados de grafo está associada às limitações de infraestrutura dela e geralmente exigem um alto grau de manutenção para garantir sua operação. Como um serviço totalmente gerenciado, o Cosmos DB acaba com a necessidade de gerenciar máquinas virtuais, atualizar o software de tempo de execução, gerenciar a fragmentação ou a replicação ou lidar com atualizações de camadas de dados complexas. Cada grafo é salvo em backup automaticamente e protegido contra falhas regionais. Esse gerenciamento permite que os desenvolvedores se concentrem no fornecimento de valor para o aplicativo em vez de operar e gerenciar os bancos de dados de grafo deles.

- Indexação automática: por padrão, a API para Gremlin indexam automaticamente todas as propriedades dentro dos nós (também chamados de vértices) e das bordas no grafo e não espera nem exige nenhum esquema ou a criação de índices secundários. Para obter mais informações, confira Indexação no Azure Cosmos DB.

- Compatibilidade com o Apache TinkerPop: a API para Gremlin dá suporte ao padrão Apache TinkerPop de software livre. O padrão Apache TinkerPop tem um amplo ecossistema de aplicativos e bibliotecas que podem ser facilmente integradas com a API.

- Níveis ajustáveis de consistência: o Azure Cosmos DB fornece cinco níveis de consistência bem-definidos para alcançar a compensação certa entre consistência e desempenho do seu aplicativo. Para operações de consulta e leitura, o Azure Cosmos DB oferece cinco níveis de consistência diferentes: forte, desatualização limitada, sessão, prefixo constante e eventual. Esses níveis de consistência granulares e bem-definidos permitem que você faça compensações seguras entre consistência, disponibilidade e latência. Para obter mais informações, consulte níveis ajustáveis de consistência de dados no Azure Cosmos DB.

Cenários comuns da API para Gremlin
Veja alguns cenários em que o suporte para grafo do Azure Cosmos DB pode ser útil:

Redes sociais/Cliente 365: combinando dados sobre seus clientes e as interações deles com outras pessoas, você pode desenvolver experiências personalizadas, prever o comportamento do cliente ou conectar pessoas com interesses semelhantes. O BD Cosmos do Azure pode ser usado para gerenciar redes sociais e monitorar dados e preferências do cliente.

Mecanismos de recomendação: esse cenário costuma ser usado no setor de varejo. Combinando informações sobre produtos, usuários e interações do usuário, como compras, navegação ou a classificação de um item, você pode criar recomendações personalizadas. O Azure Cosmos DB, com sua baixa latência, dimensionamento elástico e suporte para grafo nativo, é ideal para esses cenários.

Geoespacial: muitos aplicativos de telecomunicações, logística e planejamento de viagens precisam encontrar um local de interesse em uma área específica ou localizar a rota mais curta/ideal entre dois locais. O BD Cosmos do Azure é uma solução natural para esses problemas.

Internet das Coisas: com a rede e as conexões entre os dispositivos IoT modelados como um grafo, você pode criar uma melhor compreensão do estado de seus dispositivos e ativos. Você também pode saber mais como as alterações em uma parte da rede podem afetar potencialmente outra parte.

Introdução aos bancos de dados de grafo
Os dados da forma como aparecem no mundo real são conectados naturalmente. A modelagem de dados tradicional se concentra em definir as entidades separadamente e computar as relações delas no runtime. Embora esse modelo tenha suas vantagens, dados altamente conectados podem ser desafiadores de gerenciar em conformidade com as restrições deles.

Por sua vez, uma abordagem de banco de dados de grafo se baseia em manter relações na camada de armazenamento,o que leva a operações de recuperação de grafo altamente eficientes. A API para Gremlin dá suporte ao modelo de grafo de propriedades.

Objetos de grafo de propriedade
Um grafo de propriedade é uma estrutura composta por vértices e bordas. Ambos os objetos têm um número arbitrário de pares chave-valor como propriedades.

Vértices/nós: os vértices denotam entidades individuais, como uma pessoa, um lugar ou um evento.

Bordas/relações: as bordas indicam relações entre os vértices. Por exemplo, uma pessoa pode conhecer outra pessoa, estar envolvida em um evento ou ter estado recentemente em um local.

Propriedades: as propriedades expressam informações (ou metadados) sobre os vértices e as bordas. Pode haver qualquer número de propriedades nos vértices ou nas bordas e elas podem ser usadas para descrever e filtrar os objetos em uma consulta. As propriedades de exemplo incluem um vértice com um nome, uma idade e um limite com um carimbo de data/hora ou um peso.

Rótulo – Um rótulo é um nome ou o identificador de um vértice ou uma borda. Os rótulos podem agrupar vários vértices ou bordas para que todos os vértices/bordas em um grupo tenham um determinado rótulo. Por exemplo, um grafo pode ter vários vértices com o rótulo de "pessoa".

Os bancos de dados de grafo costumam ser incluídos na categoria de banco de dados de NoSQL ou não relacional, uma vez que não existe dependência no modelo de dados restrito ou de esquema. Essa falta de esquema permite modelar e armazenar estruturas conectadas de forma natural e eficiente.
