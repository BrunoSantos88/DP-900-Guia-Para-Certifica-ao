# Identificar formatos de dados

Os dados são uma coleção de fatos, como números, descrições e observações usados para registrar informações. As estruturas de dados nas quais esses dados são organizados geralmente representam entidades que são importantes para uma organização (como clientes, produtos, pedidos de vendas e assim por diante). Normalmente, cada entidade tem um ou mais atributos ou características (por exemplo, um cliente pode ter um nome, um endereço, um número de telefone e assim por diante).

Podemos classificar os dados como estruturados, semiestruturados ou não estruturados.

# Dados estruturados

Dados estruturados obedecem a um esquema fixo, portanto, todos os dados têm os mesmos campos ou propriedades. Normalmente, o esquema para entidades de dados estruturados é tabular. Em outras palavras, os dados são representados em uma ou mais tabelas que consistem em linhas para representar cada instância de uma entidade de dados e colunas para representar os atributos da entidade. Por exemplo, a imagem a seguir mostra representações de dados tabulares para as entidades Customer e Product.



# Dados semiestruturados
Dados semiestruturados são informações que têm alguma estrutura, mas que permitem alguma variação entre instâncias da entidade. Por exemplo, embora a maioria dos clientes possa ter um endereço de email, alguns podem ter vários endereços de email e outros podem não ter nenhum.

Um formato comum para dados semiestruturados é o JSON (JavaScript Object Notation). O exemplo a seguir mostra um par de documentos JSON que representam informações do cliente. Cada documento do cliente inclui informações de endereço e de contato, mas os campos específicos variam entre os clientes.

Exemplo. </p>
// Customer 1
{
  "firstName": "Joe",
  "lastName": "Jones",
  "address":
  {
    "streetAddress": "1 Main St.",
    "city": "New York",
    "state": "NY",
    "postalCode": "10099"
  },
  "contact":
  [
    {
      "type": "home",
      "number": "555 123-1234"
    },
    {
      "type": "email",
      "address": "joe@litware.com"
    }
  ]
}

// Customer 2
{
  "firstName": "Samir",
  "lastName": "Nadoy",
  "address":
  {
    "streetAddress": "123 Elm Pl.",
    "unit": "500",
    "city": "Seattle",
    "state": "WA",
    "postalCode": "98999"
  },
  "contact":
  [
    {
      "type": "email",
      "address": "samir@northwind.com"
    }
  ]
}

# Dados não estruturados
Nem todos os dados são estruturados ou até mesmo semiestruturados. Por exemplo, documentos, imagens, dados de áudio e vídeo e arquivos binários podem não ter uma estrutura específica. Esse tipo de dados é conhecido como dados não estruturados.

# Armazenamentos de dados

As organizações normalmente armazenam dados em formato estruturado, semiestruturado ou não estruturado para registrar detalhes de entidades (por exemplo, clientes e produtos), eventos específicos (como transações de vendas) ou outras informações em documentos, imagens e outros formatos. Os dados armazenados podem ser recuperados para análise e relatórios posteriormente.

Há duas categorias amplas de armazenamento de dados comuns em uso:

Armazenamentos de arquivos
Bancos de dados
Exploraremos esses dois tipos de armazenamento de dados nos tópicos subsequentes.

# Explorar o armazenamento de arquivos

A capacidade de armazenar dados em arquivos é um elemento básico de qualquer sistema computacional. Os arquivos podem ser armazenados em sistemas de arquivos locais no disco rígido do seu PC e em mídia removível, como unidades USB. Mas, na maioria das organizações, arquivos de dados importantes são armazenados de maneira centralizada em algum tipo de sistema de armazenamento de arquivos compartilhado. Cada vez mais, esse local de armazenamento central está sendo hospedado na nuvem, possibilitando um armazenamento econômico, seguro e confiável para grandes volumes de dados.

O formato de arquivo específico usado para armazenar dados depende de vários fatores, incluindo:

O tipo de dados que está sendo armazenado (estruturado, semiestruturado ou não estruturado).
Os aplicativos e serviços que precisarão ler, gravar e processar os dados.
A necessidade de que os arquivos de dados sejam legíveis por seres humanos ou otimizados para armazenamento e processamento eficientes.
Alguns formatos de arquivo comuns são discutidos abaixo.

# Arquivos de texto delimitado
Geralmente, os dados são armazenados em formato de texto sem formatação com delimitadores de campo e terminadores de linha específicos. O formato mais comum para dados delimitados é CSV (valores separados por vírgula) nos quais os campos são separados por vírgulas e as linhas terminam com um retorno de carro/nova linha. Opcionalmente, a primeira linha pode incluir os nomes de campo. Outros formatos comuns incluem TSV (valores separados por tabulação) e delimitado por espaço (em que as tabulações ou os espaços são usados para separar campos) e dados de largura fixa em que a cada campo é alocado um número fixo de caracteres. O texto delimitado é uma boa opção para dados estruturados que precisam ser acessados por uma ampla variedade de aplicativos e serviços em um formato legível.

O seguinte exemplo mostra dados de clientes em formato delimitado por vírgulas:

FirstName,LastName,Email
Joe,Jones,joe@litware.com
Samir,Nadoy,samir@northwind.com
