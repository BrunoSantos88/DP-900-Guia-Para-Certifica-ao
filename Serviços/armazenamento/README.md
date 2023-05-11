# Armazenamento do Azure

Azure Storage logo O Armazenamento do Azure é um serviço principal do Azure que permite armazenar dados em:

- Contêineres de blobs – armazenamento escalonável e econômico para arquivos binários.
Compartilhamentos de arquivos – compartilhamentos de arquivos de rede, semelhante ao que normalmente é encontrado nas redes corporativas.
Tabelas – armazenamento de chave-valor para aplicativos que precisam ler e gravar valores de dados rapidamente.
Os engenheiros de dados usam o Armazenamento do Azure para hospedar data lakes – armazenamentos de blobs com um namespace hierárquico que permite que os arquivos sejam organizados em pastas em um sistema de arquivos distribuído.

# Explorar o Armazenamento de Blobs do Azure

O Armazenamento de Blobs do Azure é um serviço que permite armazenar grandes quantidades de dados não estruturados como objetos grandes binários, ou blobs, na nuvem. Os blobs são uma maneira eficiente de armazenar arquivos de dados em um formato otimizado para armazenamento baseado em nuvem, e os aplicativos podem lê-los e gravá-los usando a API de armazenamento de blobs do Azure.

Um contêiner de armazenamento de blobs do Azure com dois blobs

Em uma conta de armazenamento do Azure, você armazena blobs em contêineres. Um contêiner oferece uma maneira prática de agrupar blobs relacionados. Você controla quem pode ler e gravar blobs dentro de um contêiner no nível do contêiner.

Dentro de um contêiner, você pode organizar blobs em uma hierarquia de pastas virtuais, semelhante a arquivos em um sistema de arquivos em disco. No entanto, por padrão, essas pastas são simplesmente uma maneira de usar um caractere "/" em um nome de blob para organizar os blobs em namespaces. As pastas são puramente virtuais, e você não pode executar operações no nível da pasta para controlar o acesso ou executar operações em massa.

O Armazenamento de Blobs do Azure é compatível com três tipos diferentes de blob:

# Blobs de blocos. 

- Um blob de blocos é tratado como um conjunto de blocos. Cada bloco pode variar em tamanho, até 100 MB. Um blob de blocos pode conter até 50 mil blocos, fornecendo um tamanho máximo de mais de 4,7 TB. O bloco é a menor quantidade de dados que podem ser lidos ou gravados como uma unidade individual. Os blobs de blocos são mais bem usados para armazenar objetos binários, grandes e discretos que são alterados com pouca frequência.
 
# Blobs de páginas. 

- Um blob de páginas é organizado como uma coleção de páginas de tamanho fixo de 512 bytes. Um blob de páginas é otimizado para dar suporte a operações de leitura e gravação aleatórias; você pode buscar e armazenar dados para uma página, se necessário. Um blob de páginas pode conter até 8 TB de dados. O Azure usa blobs de páginas para implementar o armazenamento em disco virtual para máquinas virtuais.

# Blobs de acréscimo
- Blobs de acréscimo. Um blob de acréscimo é um blob de blocos otimizado para dar suporte a operações de acréscimo. Você só pode adicionar blocos ao final de um blob de acréscimo; não há suporte à atualização ou à exclusão de blocos existentes. Cada bloco pode variar em tamanho, até 4 MB. O tamanho máximo de um blob de acréscimo é de mais de 195 GB.

# O Armazenamento de Blobs fornece três camadas de acesso, que ajudam a balancear a latência de acesso e o custo de armazenamento:

# CAMADA HOT
- A camada Quente é a padrão. Você usa essa camada para blobs que são acessados com frequência. Os dados de blob são armazenados em mídia de alto desempenho.

# Camada Cool
- A camada de acesso esporádico tem desempenho inferior e incorre em custos de armazenamento reduzidos em comparação com a camada de acesso frequente. Use a camada Fria para dados que são acessados com pouca frequência. É comum que blobs recém-criados sejam acessados inicialmente com frequência, mas com o passar do tempo, ela diminui. Nessas situações, você pode criar o blob na camada Quente, mas migrá-lo para a camada Fria mais tarde. Você pode migrar um blob da camada Fria de volta para a camada Quente.

# Camada Arquivo
- A camada de acesso aos arquivos oferece o menor custo de armazenamento, mas com maior latência. A camada Arquivos se destina a dados históricos que não devem ser perdidos, mas é necessária apenas raramente. Os blobs na camada Arquivos são efetivamente armazenados em um estado offline. A latência de leitura típica para as camadas Quente e Fria é de alguns milissegundos, mas, para a camada Arquivos, pode levar horas para que os dados fiquem disponíveis. Para recuperar um blob da camada Arquivos, você precisa alterar a camada de acesso para Quente ou Fria. Em seguida, o blob será reidratado. Você poderá ler o blob somente quando o processo de reidratação estiver concluído.

- Você pode criar políticas de gerenciamento de ciclo de vida para blobs em uma conta de armazenamento. Uma política de gerenciamento do ciclo de vida pode migrar automaticamente um blob da camada Quente para a Fria e para a camada Arquivos, pois ele envelhece e é usado com menos frequência (a política é baseada no número de dias desde a modificação). Uma política de gerenciamento do ciclo de vida também pode ser organizada para excluir blobs desatualizados.
