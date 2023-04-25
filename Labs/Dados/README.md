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