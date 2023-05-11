# Descrever serviços do Azure para bancos de dados de código aberto

Além dos serviços de SQL do Azure, há serviços de dados do Azure disponíveis para outros sistemas de bancos de dados relacionais populares, incluindo MySQL, MariaDB e PostgreSQL. O propósito desses serviços é permitir que as organizações que os usam em aplicativos locais migrem para o Azure rapidamente, sem fazer alterações significativas em seus aplicativos.

O que são MySQL, MariaDB e PostgreSQL?
MySQL, MariaDB e PostgreSQL são sistemas de gerenciamento de banco de dados relacionais personalizados para diferentes especializações.

O MySQL começou como um sistema de gerenciamento de banco de dados de software livre simples de usar. É o principal banco de dados relacional de código aberto para os aplicativos da pilha LAMP (Linux, Apache, MySQL e PHP). Ele está disponível em várias edições; Community, Standard e Enterprise. A Community Edition está disponível gratuitamente e tem sido historicamente popular como um sistema de gerenciamento de banco de dados para aplicativos Web, em execução no Linux. Também há versões disponíveis para Windows. A Edição Standard tem um desempenho mais alto e usa uma tecnologia diferente para armazenar dados. A Edição Enterprise fornece um conjunto abrangente de ferramentas e recursos, incluindo segurança, disponibilidade e escalabilidade aprimoradas. As edições Standard e Enterprise são as versões usadas com mais frequência pelas organizações comerciais, embora essas versões do software não sejam gratuitas.

O MariaDB é um sistema de gerenciamento de banco de dados mais recente, criado pelos desenvolvedores originais do MySQL. Desde então, o mecanismo de banco de dados foi reescrito e otimizado para aprimorar o desempenho. O MariaDB tem compatibilidade com o Oracle Database (outro sistema de gerenciamento de banco de dados comercial popular). Um recurso notável do MariaDB é o suporte interno para dados temporais. Uma tabela pode conter várias versões de dados, permitindo que um aplicativo consulte os dados como eles apareciam em algum momento no passado.

O PostgreSQL é um banco de dados de objetos híbrido e relacional. É possível armazenar dados em tabelas relacionais, mas um banco de dados PostgreSQL também permite que você armazene tipos de dados personalizados, com propriedades não relacionais próprias. O sistema de gerenciamento de banco de dados é extensível. Você pode adicionar módulos de código ao banco de dados, que pode ser executado por consultas. Outro recurso importante é a capacidade de armazenar e manipular dados geométricos, como linhas, círculos e polígonos.

O PostgreSQL tem uma linguagem de consulta própria chamada pgsql. É uma variante da linguagem de consulta relacional padrão, SQL, com recursos que permitem escrever procedimentos armazenados executados dentro do banco de dados.

Banco de Dados do Azure para MySQL
Logotipo do Banco de Dados do Azure para MySQLO Banco de Dados do Azure para MySQL é uma implementação do MySQL na nuvem do Azure, baseada na Community Edition do MySQL.

O serviço do Banco de Dados do Azure para MySQL inclui alta disponibilidade sem custo adicional e escalabilidade de acordo com a necessidade. Você paga apenas pelo que usa. É possível fazer backups automáticos com restauração pontual.

O servidor fornece segurança de conexão para impor regras de firewall e, opcionalmente, exigir conexões SSL. Muitos parâmetros de servidor permitem definir as configurações do servidor, como modos de bloqueio, número máximo de conexões e tempos limite.

O Banco de Dados do Azure para MySQL fornece um sistema de banco de dados global que pode ser dimensionado para grandes bancos de dados sem a necessidade de gerenciar hardware, componentes de rede, servidores virtuais, patches de software e outros componentes subjacentes.

Determinadas operações não estão disponíveis no Banco de Dados do Azure para MySQL. Essas funções se encarregam principalmente da segurança e da administração. O Azure gerencia esses aspectos do próprio servidor de banco de dados.

Benefícios do Banco de Dados do Azure para MySQL
Os seguintes recursos estão disponíveis no Banco de Dados do Azure para MySQL:

Recursos internos de alta disponibilidade.
Desempenho previsível.
Dimensionamento fácil que responde rapidamente à demanda.
Proteção dos dados, em repouso e em movimento.
Backups automáticos e restauração pontual dos últimos 35 dias.
Segurança de nível empresarial e conformidade com a legislação.
O sistema usa o preço pago conforme o uso para que você pague apenas pelo que usar.

Os servidores do Banco de Dados do Azure para MySQL oferecem recursos de monitoramento para adicionar alertas e ver métricas e logs.

Banco de Dados do Azure para MariaDB
Logotipo do Banco de Dados do Azure para MariaDBO Banco de Dados do Azure para MariaDB é uma implementação do sistema de gerenciamento de banco de dados MariaDB adaptado para execução no Azure. Baseia-se na Community Edition do MariaDB.

O banco de dados é totalmente gerenciado e controlado pelo Azure. Depois de provisionar o serviço e transferir seus dados, o sistema não requer quase nenhuma administração adicional.

Benefícios do Banco de Dados do Azure para MariaDB
O Banco de Dados do Azure para MariaDB oferece:

Alta disponibilidade interna sem nenhum custo adicional.
Desempenho previsível, com preços pré-pagos inclusivos.
Dimensionamento em segundos, conforme o necessário.
Proteção para dados confidenciais em repouso e em movimento.
Backups automáticos e restauração pontual por até 35 dias.
Segurança e conformidade de nível empresarial.
Banco de Dados do Azure para PostgreSQL
Logotipo do Banco de Dados do Azure para PostgreSQLSe preferir o PostgreSQL, você poderá escolher o Banco de Dados do Azure para PostgreSQL para executar uma implementação de PaaS do PostgreSQL na nuvem do Azure. Esse serviço fornece os mesmos benefícios de disponibilidade, desempenho, dimensionamento, segurança e administração que o MySQL.

Alguns recursos dos bancos de dados PostgreSQL locais não estão disponíveis no Banco de Dados do Azure para PostgreSQL. Esses recursos se encarregam principalmente das extensões que os usuários podem adicionar a um banco de dados para executar tarefas especializadas, como escrever procedimentos armazenados em várias linguagens de programação (além de pgsql, que está disponível) e interagir diretamente com o sistema operacional. Há compatibilidade com um conjunto básico de extensões usadas com mais frequência e a lista de extensões disponíveis está sob análise contínua.

Banco de Dados do Azure para PostgreSQL Servidor Flexível
A opção de implantação de servidor flexível para PostgreSQL é um serviço de banco de dados totalmente gerenciado. Ele fornece um alto nível de controle e personalizações de configuração do servidor, além de oferecer melhores controles de otimização de custo.

Benefícios do Banco de Dados do Azure para PostgreSQL
O Banco de Dados do Azure para PostgreSQL é um serviço altamente disponível. Ele contém mecanismos internos de detecção de falha e failover.

Os usuários do PostgreSQL conhecerão a ferramenta pgAdmin, que você pode usar para gerenciar e monitorar um banco de dados PostgreSQL. Você pode continuar a usar essa ferramenta para se conectar ao Banco de Dados do Azure para PostgreSQL. No entanto, alguns recursos voltados para o servidor, como executar backup e restauração do servidor, não estão disponíveis porque o servidor é gerenciado e mantido pela Microsoft.

O Banco de Dados do Azure para PostgreSQL registra informações sobre as consultas executadas em bancos de dados no servidor e as salva em um banco de dados chamado azure_sys. Consulte a exibição query_store.qs_view para ver essas informações e usá-las para monitorar as consultas que os usuários estão executando. Essas informações podem se mostrar valiosas se você precisa ajustar as consultas executadas por seus aplicativos.
