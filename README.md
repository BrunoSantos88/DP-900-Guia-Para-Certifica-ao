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
