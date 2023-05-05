# Bancos de dados

Aplica-se a:SQL ServerBanco de Dados SQL do AzureInstância Gerenciada de SQL do Azure

Um banco de dados no SQL Server é composto de uma coleção de tabelas que armazenam um conjunto específico de dados estruturados. Uma tabela contém uma coleção de linhas, também chamadas de registros ou tuplas, e colunas, também chamadas de atributos. Cada coluna da tabela é projetada para armazenar um determinado tipo de informação, por exemplo, datas, nomes, valores em dinheiro e números.

# Informações básicas sobre bancos de dados
Um computador pode ter uma ou mais de uma instância de SQL Server instalada. Cada instância de SQL Server pode conter um ou muitos bancos de dados. Dentro de um banco de dados, há um ou vários grupos de propriedade de objeto denominados esquemas. Em cada esquema, há objetos de banco de dados como tabelas, exibições e procedimentos armazenados. Alguns objetos, como certificados e chaves assimétricas, estão contidos no banco de dados, mas não estão contidos em um esquema. Para obter mais informações sobre como criar tabelas, consulte Tabelas.

- SQL Server bancos de dados são armazenados no sistema de arquivos em arquivos. Os arquivos podem ser agrupados em grupos de arquivos. Para obter mais informações sobre como os arquivos e grupos de arquivos, consulte Arquivos e grupos de arquivos do banco de dados.

- Quando as pessoas obtêm acesso a uma instância de SQL Server elas são identificadas como um logon. Quando as pessoas obtiverem acesso a um banco de dados, elas serão identificadas como um usuário de banco de dados. Um usuário de banco de dados pode ser baseado em um logon. Se forem habilitados bancos de dados independentes, um usuário de banco de dados não baseado em logon poderá ser criado. Para obter mais informações sobre usuários, consulte CREATE USER (Transact-SQL).

- Um usuário que tem acesso a um banco de dados pode receber permissão para acessar os objetos no banco de dados. Embora possam ser concedidas permissões a usuários individuais, é recomendável criar funções de banco de dados, adicionando os usuários de banco de dados às funções, e conceder permissão de acesso às funções. A concessão de permissões a funções, e não a usuários, faz com que seja mais fácil manter as permissões consistentes e compreensíveis à medida que o número de usuários aumenta e muda continuamente. Para obter mais informações sobre permissões de funções, consulte CREATE ROLE (Transact-SQL) e Entidades de Segurança (Mecanismo de Banco de Dados).

# Trabalhando com bancos de dados
A maioria das pessoas que trabalham com bancos de dados usa a ferramenta SQL Server Management Studio. A ferramenta Management Studio tem uma interface gráfica do usuário para criar bancos de dados e os objetos nos bancos de dados. O Management Studio também tem um editor de consultas para interagir com bancos de dados escrevendo instruções Transact-SQL. O Management Studio pode ser instalado do SQL Server disco de instalação ou baixado do MSDN. Para obter mais informações sobre SQL Server Management Studio ferramenta, consulte SQL Server Management Studio (SSMS).

# Descrever os serviços e recursos do SQL do Azure

- SQL do Azure é um termo coletivo para uma família de serviços de banco de dados baseados no Microsoft SQL Server no Azure. Os serviços específicos de SQL do Azure incluem:

- SQL Server em VMs (Máquinas Virtuais) do Azure – uma máquina virtual em execução no Azure com uma instalação do SQL Server. O uso de uma VM torna essa opção uma solução de IaaS (infraestrutura como serviço) que virtualiza a infraestrutura de hardware para computação, armazenamento e rede no Azure, tornando-a uma ótima opção para migração "lift-and-shift" de instalações locais existentes do SQL Server para a nuvem.
Instância Gerenciada de SQL do Azure – uma opção de PaaS (plataforma como serviço) que fornece quase 100% de compatibilidade com instâncias de SQL Server locais, abstraindo o hardware e o sistema operacional subjacentes. O serviço inclui gerenciamento automatizado de atualizações de software, backups e outras tarefas de manutenção, reduzindo a carga administrativa do suporte a uma instância de servidor de banco de dados.
- Banco de Dados SQL do Azure – um serviço de banco de dados de PaaS totalmente gerenciado e altamente escalonável projetado para a nuvem. Esse serviço inclui os principais recursos de nível de banco de dados do SQL Server local e é uma boa opção se você precisa criar um aplicativo na nuvem.
- SQL do Azure no Edge – um mecanismo SQL que é otimizado para cenários de IoT (Internet das Coisas) que precisam trabalhar com transmissão de dados de séries temporais.
