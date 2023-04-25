# DP-900-Guia-Para-Certificação
-Curso ministrado pelo SENAI,usando conceitos de Learning path.

Link roteiro DP-900: https://learn.microsoft.com/pt-br/training/browse/?terms=DP-900&resource_type=learning%20path&subjects=data-ai


# Qual o significado de OLTP e OLAP?
Apesar de apresentarem nomes parecidos, seus conceitos e aplicações são bem diferentes. Portanto, entender a função de cada um é fundamental para utilizá-los corretamente.

OLTP ou Online Transaction Processing (Processamento de Transações Online, em português) serve para designar os sistemas operacionais com dados transacionais. 

Além de fornecerem assistência para as atividades na visão operacional, o OLTP processa dados dos diversos sistemas com informações variadas da companhia.

Por outro lado, o OLAP ou Online Analytical Processing (Processamento Analítico Online), é uma habilidade para executar dentro do Data Warehouse e realizar análises dos grandes volumes de dados. 

# Qual é a diferença entre batch e stream?
O batch é um lote de pontos de dados que foram agrupados em um intervalo de tempo específico. Outro termo frequentemente usado para isso é uma janela de dados. Já o processamento de dados em stream lida com dados contínuos e é essencial para transformar de grandes a rápidos.

Ambos os modelos são valiosos e cada um pode ser usado para tratar de diferentes casos de uso. Embora o modelo de processamento em batch exija um conjunto de dados coletados ao longo do tempo, o processamento de stream requer que os dados sejam inseridos em uma ferramenta de análise, geralmente, em lotes menores e em tempo real.

O processamento em batch é usado com frequência quando se lida com grandes volumes de dados ou fontes de dados de sistemas legados, em que não é possível entregar dados em fluxos. Ele também, por definição, exige que todos os dados necessários para o lote sejam carregados em algum tipo de armazenamento, um banco de dados ou sistema de arquivos para serem processados.

Nesse caso, é comum acontecer que as equipes de TI fiquem paradas esperando que todos os dados sejam carregados antes de iniciar a fase de análise.

O stream também podem estar envolvido no processamento de grandes quantidades de dados, mas o batch funciona melhor quando você não precisa de análises em tempo real.

Como o processamento stream é responsável pelo processamento de dados em movimento e pelo rápido fornecimento de análise, ele gera resultados quase instantâneos usando plataformas de

# Quando escolher batch ou stream?
Se você não tem uma longa história de trabalho com o processamento de stream, você pode perguntar: “por que não podemos apenas o batch como antes?”. Você certamente pode, mas se tiver enormes volumes de dados, não é uma questão de quando você precisar extraí-los, mas quando precisará usá-los.

As empresas veem os dados em tempo real como um divisor de águas, mas ainda pode ser um desafio chegar lá sem as ferramentas adequadas, principalmente, porque elas precisam trabalhar com volumes, variedades e tipos de dados cada vez maiores de diversos sistemas, como mídias sociais.

Normalmente, as organizações querem ter processos de dados mais ágeis para poderem passar da imaginação para a inovação mais rapidamente e responder às ameaças da concorrência.

Por exemplo, os dados enviados dos sensores de uma turbina eólica estão sempre ligados. Assim, o fluxo de dados é ininterrupto e flui o tempo todo. Uma abordagem em batch aqui seria obsoleta, pois não há início ou parada do fluxo. Esse é um caso de uso perfeito em que o processamento de stream é o caminho a percorrer.

O processamento de dados em batch e stream são dois modelos diferentes — não é uma questão de escolher um sobre o outro, é sobre ser assertivo e determinar qual é o melhor para cada caso de uso.


# O que é processamento em lote?
O processamento em lote é quando um computador processa várias tarefas reunidas em um grupo. Ele foi projetado para ser um processo totalmente automatizado, sem intervenção humana. Também pode ser chamado de automação de carga de trabalho (WLA) e agendamento de tarefas.

O processamento em lote é uma maneira incrivelmente econômica de processar grandes quantidades de dados em um curto período de tempo. Uma vez iniciado o processo, o computador só para quando descobre um erro ou anormalidade, notificando o funcionário ou gerente apropriado.


# ETL (extração, transformação e carregamento)
Synapse Analytics
Data Factory
Um problema comum que as organizações enfrentam é como coletar dados de várias fontes em vários formatos. Depois, você precisa movê-los para um ou mais armazenamentos de dados. O destino pode não ser o mesmo tipo de armazenamento de dados que a origem. Muitas vezes, o formato é diferente ou os dados precisam ser formatados ou limpos antes de serem carregados no destino final.

Várias ferramentas, serviços e processos foram desenvolvidos ao longo dos anos para ajudar a solucionar esses desafios. Qualquer que seja o processo utilizado, há uma necessidade comum de coordenar o trabalho e aplicar algum nível de transformação de dados dentro do pipeline de dados. As seções a seguir destacam os métodos comuns usados para executar essas tarefas.
