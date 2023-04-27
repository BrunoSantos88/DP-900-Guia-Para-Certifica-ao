# Bancos de dados de grafo

Um banco de dados de gráfico armazena dois tipos de informações, nós e bordas. As bordas especificam os relacionamentos entre os nós. Tanto os nós quanto as bordas podem ter propriedades que fornecem informações sobre o nó ou a borda questão, semelhante às colunas em uma tabela. As bordas também podem ter uma direção indicando a natureza do relacionamento.

Os bancos de dados de grafo podem executar consultas com eficiência na rede de nós e bordas, além de analisar os relacionamentos entre as entidades. O diagrama a seguir mostra o banco de dados de pessoal de uma organização estruturado como um grafo. As entidades são funcionários e departamentos, e as bordas indicam os relacionamentos de subordinação e os departamentos em que os funcionários trabalham.

# Diagrama de um banco de dados de documentos

Essa estrutura simplifica a execução de consultas como "Encontrar todos os funcionários que são subordinados diretos ou indiretos de Marina" ou "Quem trabalha no mesmo departamento que Júlio?". Para grafos grandes com muitas entidades e relacionamentos, você pode executar análises complexas rapidamente. Muitos bancos de dados de gráficos fornecem uma linguagem de consulta que você pode utilizar para percorrer uma rede de relacionamentos de forma eficiente.

# Serviços do Azure

Azure Cosmos DB for Apache Gremlin | (Linha de base de segurança)
SQL Server | (Linha de base de segurança)

#Carga de trabalho

Os relacionamentos complexos entre os itens de dados envolvem vários saltos entre os itens de dados relacionados.
A relação entre os itens de dados são dinâmicas e mudam com o passar do tempo.
As relações entre objetos são de primeira classe, sem precisar de chaves estrangeiras e ingressos para serem percorridas.

# Tipo de dados

Nós e relacionamentos.
Nós são semelhantes às linhas da tabela ou documentos JSON.
As relações são tão importantes quanto os nós e são expostas diretamente na linguagem de consulta.
Objetos de composição, como uma pessoa com vários números de telefone, tendem a ser divididos em nós menores combinado com relações navegáveis

# Exemplos
Quadros da organização
Gráficos sociais
Detecção de fraude
Mecanismos de recomendação

Exemplo: </p>
</p>
<img src="https://user-images.githubusercontent.com/91704169/234874515-16b1b4bb-0ab8-4c55-a0a2-b8aa4c4c3411.png" width="1000px" align="centter" alt="planos">
