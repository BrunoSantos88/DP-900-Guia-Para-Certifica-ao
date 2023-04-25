# ETL (extração, transformação e carregamento)
Synapse Analytics
Data Factory
Um problema comum que as organizações enfrentam é como coletar dados de várias fontes em vários formatos. Depois, você precisa movê-los para um ou mais armazenamentos de dados. O destino pode não ser o mesmo tipo de armazenamento de dados que a origem. Muitas vezes, o formato é diferente ou os dados precisam ser formatados ou limpos antes de serem carregados no destino final.

Várias ferramentas, serviços e processos foram desenvolvidos ao longo dos anos para ajudar a solucionar esses desafios. Qualquer que seja o processo utilizado, há uma necessidade comum de coordenar o trabalho e aplicar algum nível de transformação de dados dentro do pipeline de dados. As seções a seguir destacam os métodos comuns usados para executar essas tarefas.

# ELT (extração, carregamento e transformação)
O ELT (extração, carregamento e transformação) difere do ETL somente no local em que ocorre a transformação. No pipeline de ELT, a transformação ocorre no armazenamento de dados de destino. Em vez de usar um mecanismo de transformação separado, as funcionalidades de processamento do armazenamento de dados de destino são usadas para transformar os dados. Isso simplifica a arquitetura pela remoção do mecanismo de transformação do pipeline. Outro benefício dessa abordagem é que o dimensionamento do armazenamento de dados de destino também dimensiona o desempenho do pipeline ELT. No entanto, o ELT só funciona bem quando o sistema de destino é poderoso o suficiente para transformar os dados com eficiência.


Exemplo: </p>
</p>
<img src="https://learn.microsoft.com/pt-br/training/wwl-data-ai/get-started-ai-fundamentals/media/machine-learn.gif" width="1000px" align="centter" alt="planos">
