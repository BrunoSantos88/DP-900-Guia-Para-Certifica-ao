# O que é um data warehouse?
Primeiro, vamos definir o que é um data warehouse e por que você pode querer usar um para sua organização.

Um data warehouse é um repositório centralizado que armazena dados estruturados (tabelas de banco de dados, planilhas do Excel) e dados semiestruturados (arquivos XML, páginas da Web) para fins de relatório e análise. Os dados fluem de uma variedade de fontes, como sistemas de ponto de venda, aplicativos de negócios e bancos de dados relacionais, e geralmente são limpos e padronizados antes de chegar ao depósito. Como um data warehouse pode armazenar grandes quantidades de informações, ele fornece aos usuários acesso fácil a uma grande quantidade de dados históricos, que podem ser usados para mineração de dados, visualização de dados e outras formas de relatórios de business intelligence.

# Conceito de Data Warehouse
O Data Warehouse é um armazém de dados ou repositório de dados. Trata-se de uma estrutura de armazenamento que guarda dados em um formato estruturado para facilitar consultas e análises. Não é somente um conjunto de dados, mas um conjunto disposto para facilitar o uso por ferramentas analíticas.

Nesse sentido, um warehouse se destaca como uma opção para coleta e tratamento do Big Data. Além disso, é uma importante ferramenta para projetos de Data Science, servindo como uma base estrutural com dados para treinamento de algoritmos.

Em suma, o DW registra os dados e os históricos associados para possibilitar a melhor tomada de decisão de gestores. Dessa forma, permite responder a perguntas importantes do negócio, como quantas vendas foram feitas no mês X, quantos clientes desistiram do serviço no mês passado e outras questões relacionadas.

O time de marketing, por exemplo, pode olhar para dados de acesso do site e do blog para pensar em abordagens de SEO ou melhorias consideráveis na personalização do conteúdo. O marketing de conteúdo e o email marketing também são favorecidos com o uso do warehouse como um repositório central de dados, uma vez que é possível o ajuste das estratégias constantemente.

# Conheça a arquitetura de um Data Warehouse
Vamos aprofundar no conceito de um DW. Agora, falaremos sobre a arquitetura que compõe essa estrutura.

Inicialmente, vale destacar que a arquitetura varia muito a depender da robustez e complexidade do DW. Os elementos que citaremos a seguir são organizados em camadas que realizam algum tipo de função, sendo que quanto mais camadas existem, mais complexo é o warehouse.

Em uma organização em três camadas, por exemplo, temos uma camada inicial para a extração dos dados, uma segunda para limpeza e outra para consultas e análises. Assim como podemos ter um Data Warehouse simples, com apenas uma camada.

Vamos então destrinchar componentes que fazem parte de uma arquitetura de DW de tês camadas.

# Bancos de dados
Bancos de dados são coleções organizadas de dados que permitem leitura e escrita, com acesso e recuperação rápidos. Geralmente, surgem em um formato relacional, o que significa que organizam os dados em tabelas (linhas e colunas) que se relacionam logicamente entre si.

Eles fazem parte do conceito de warehouse, sendo um fundamento para esse conceito. Em suma, um DW é um conjunto de bancos de dados com algumas funcionalidades a mais.

# ETL
Em seguida, na arquitetura de um armazém de dados, temos ferramentas ETL. O termo significa “extrair, transformar e carregar”. Trata-se de uma solução que cuida dos dados antes que eles sejam carregados no warehouse.

Primeiro, se extrai os dados de fontes transacionais ou não, como CRM e ERP. Depois, temos a limpeza e a formatação dos dados, com padronização, eliminação de itens faltantes, gestão dos nomes dos arquivos etc. Em seguida, os dados são carregados para o repositório.

Uma solução ETL é essencial para a noção de warehouse, pois é ela que garante a qualidade e o esquema dos dados que entram. Desse modo, é possível utilizar os dados para seus fins analíticos na outra ponta.

# Metadados
Quando falamos em estruturas de armazenamento de dados, precisamos citar a importância dos metadados. Eles descrevem os dados armazenados e auxiliam no trabalho técnico dos desenvolvedores e gestores que dominam essas informações. Os metadados permitem compreender melhor o que está no DW, de modo que esses dados sejam úteis para os fins estabelecidos.

# Data Marts
Outro elemento importante nessas estruturas é o Data Mart. É um conjunto de dados específico para uma análise segmentada e departamental, sendo, portanto, o resultado da divisão dos dados do warehouse em uma camada posterior. Os DMs são pequenos subgrupos de dados que dizem respeito apenas a um determinado setor, de forma a responder perguntas específicas.

Faz pleno sentido a divisão de um repositório centralizado em pequenos subgrupos posteriormente se o objetivo é a análise de dados. Uma vez que esses ativos já estão limpos e formatados, é possível então facilitar as consultas ao oferecer a cada setor os dados necessários rapidamente. Também é fundamental para controle de acesso a dados confidenciais.

# Ferramentas de acesso
Por fim, na arquitetura de um Data Warehouse, temos as ferramentas de acesso. São os sistemas que acessarão os dados dispostos no DW, de modo a efetuar as análises. Pode ser uma solução de Business Intelligence, por exemplo, com o intuito de gerar relatórios completos acerca dos dados, das métricas/indicadores e do histórico de dados. Pode ser também um projeto de Data Science.

As ferramentas de acesso correspondem à visão do usuário final, que busca os dados para visualização, criação de relatórios, mineração dos dados ou treinamento de modelos de machine learning.


# Veja as principais características de um Data Warehouse
Abaixo, apresentamos algumas das principais características de um DW. Acompanhe!

# Gestão dos dados
Uma das principais características do DW é a gestão dos dados e da mudança deles. O warehouse viabiliza uma visão histórica dos dados, em vez de somente uma visão do estado atual. Desse modo, a compreensão sobre os dados se torna ainda mais profunda, com assimilação de mais nuances.

# Integração dos dados
Outro fator é a integração dos dados. No DW, temos uma concentração de dados de diferentes fontes, que surgem em formatos distintos. Dados transacionais, dados estratégicos, de negócio etc.

Essa integração é de certa forma fundamental para fazer o melhor uso dos dados, mas também facilita a gestão deles. A centralização torna a estrutura de um DW mais complexa ao mesmo tempo em que simplifica os próximos passos a partir dele.

# Não volatilidade dos dados
Vale mencionar também a não volatilidade dos dados. Isso quer dizer que quando os dados estão no warehouse, eles permanecem persistentes e estáveis, sem mudar o seu estado. Mesmo que o DW consiga visualizar os dados em relação a outros mais antigos ou mais recentes (o histórico), os dados em si (cada unidade) permanecem inalterados.

Assim como os bancos de dados que compõem sua estrutura, um DW é fundamentalmente relacional. Isso quer dizer que lida com linhas e colunas em tabelas simples de compreender. Geralmente, os dados não relacionais precisam passar por uma esquematização antes de serem carregados no warehouse, com o apoio de ferramentas ETL.

#  Agilidade nas consultas
Justamente por organizar os dados em um formato fácil e padronizado, os warehouses favorecem consultas e análises rápidas, com um melhor desempenho do que outras estruturas. Cada membro dos diferentes departamentos consegue rapidamente responder perguntas emergentes sobre os processos e o negócio, de modo a agir de forma eficaz em tempo real.

# Dados de qualidade
Se a sua empresa precisa cuidar da qualidade dos dados e assegurar a integridade deles, um DW é uma boa opção para armazenamento. Como já falamos, a arquitetura do DW pressupõe a existência de ferramentas de limpeza dos dados, o que garante que apenas dados claros, limpos e em perfeito estado estarão disponíveis para acesso.

Essa gestão da qualidade dos dados é fundamental para estabelecer compliance com leis e normas externas de proteção e segurança, bem como regras internas de gestão e governança.

# Segurança
Atualmente, diante das estritas normas de segurança que são impostas às empresas, um DW é muito importante para ajudar a melhorar a administração dos dados e reforçar a proteção. É possível definir regras de acesso, cuidar da qualidade dos dados e manter um controle ativo do ciclo de vida dos ativos enquanto eles estão armazenados no warehouse.

Ademais, os dados concentrados facilitam as ações de segurança. Protocolos podem ser aplicados a todos de uma vez só, como uma configuração-padrão no DW.

# Visão histórica
Outro ponto de extrema relevância é a visão de dados históricos. Ou seja, como já falamos, o DW não somente registra os dados em um certo momento no tempo, como também gerencia a mudança com o tempo. Ou seja, é possível olhar para tendências temporais e analisar como os dados mudaram e como costumam mudar.

Isso é crucial para análises preditivas, por exemplo. Ao verificar tendências históricas, a empresa consegue prever comportamentos de determinadas variáveis para saber o que esperar. Da mesma forma, os dados históricos servem como base para o treinamento de modelos de machine learning.

Por outro lado, essa visão histórica também é interessante para dashboards e painéis completos de visualização. Caso o usuário final decida criar painéis para visualizar relatórios, indicadores e gráficos, ele pode explorar diferentes ângulos e obter os insights que precisa. Pode ser o time de marketing com um histórico de conversões ou o time de vendas com um histórico de vendas em determinada loja, por exemplo.

# Escalabilidade
Outra característica vantajosa de Data Warehouses é sua escalabilidade. Essa estrutura é perfeita para lidar com conjuntos crescentes de dados, gerados em tempo real, de diferentes maneiras. Com sua solução de tratamento, o DW consegue se preparar para filtrar e organizar esses dados, independentemente do tamanho deles ou do tamanho dos conjuntos em geral.

Por isso, o DW é flexível o suficiente para gerenciar o Big Data. A sua arquitetura possibilita limpar os dados, armazená-los e prepará-los para a análise rápida, de acordo com o esperado.

# Autonomia para os funcionários
Outra vantagem de um bom DW é desenvolver autonomia para todos os colaboradores. Diferentemente de outras soluções, que requerem participação ativa e exclusiva de desenvolvedores e pessoas técnicas de TI, um warehouse gera dados para que qualquer um consiga fazer análises.

Ou seja, reforça a noção de análise self-service, em que as pessoas conseguem responder suas perguntas-chave sem um grande embasamento técnico. A própria estrutura já organiza e separa os dados para facilitar relatórios e consultas, de modo que se perca menos tempo com elas, como mencionamos anteriormente.

Assim, há menos peso sobre os ombros do time de TI e as informações fluem mais rápido dentro da companhia.

# Outros benefícios que podemos mencionar:

separação do processamento analítico dos bancos de dados transacionais;
diminuição do trabalho manual;
redução de burocracia e custos;
vantagem competitiva.
O Data Warehouse é uma das mais importantes tecnologias quando falamos em armazenamento de dados para análise. Trata-se de uma solução imprescindível para gestores que desejam gerar valor e obter insights para decisões em tempo real. Assim, é possível transformar mais dados em informação útil e poderosa para o dia a dia, de modo a otimizar os processos e garantir a continuidade do negócio.

Exemplo: </p>
</p>
<img src="https://user-images.githubusercontent.com/91704169/235674570-c7b22a48-32d8-4066-8a69-b96b5101ca35.gif" width="1000px" align="centter" alt="planos">
