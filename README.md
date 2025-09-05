# portfolio_citybikes

Este é um projeto (em desenvolvimento...) com base em um dos "Capstone Projects" sugeridos pelo Google Data Analytics Professional Certificate.

Teoricamente, este seria um estudo de caso utilizando SQL, Excel e/ou R. Porém, ajustei para os meus objetivos profissionais e decidi utilizar o ambiente do Databricks para preparação e processamento dos dados, bem como criação das principais tabelas fato e dimensão.

Para a visualização dos dados eu escolhi o Power BI.

Este repositório foi dedicado a representar em foco as etapas desenvolvidas no Databricks para criação das tabelas no SQL Warehouse.

O projeto completo poderá ser consultado em meu site: https://thiagorubioli.com

### Contexto
O contexto do estudo de caso é fictício, criado pelos responsáveis pelo curso (Google e Coursera), mas os dados são reais, públicos e sob propriedade da cidade de Chicago (EUA). Mais informações sobre os dados podem ser consultadas no link: https://divvybikes.com/data-license-agreement

Sobre o estudo de caso, segue a contextualização:

"O diretor de marketing de uma empresa de aluguel/compartilhamento de bicicletas acredita que o sucesso futuro da empresa depende da maximização do número de assinaturas anuais. Portanto, sua equipe quer entender como ciclistas casuais e membros anuais usam as bicicletas de forma diferente. A partir desses insights, sua equipe desenvolverá uma nova estratégia de marketing para converter ciclistas casuais em membros anuais. Mas, primeiro, os executivos precisam aprovar suas recomendações, que devem ser respaldadas por insights e visualizações de dados profissionais."

### Perguntas
- Pergunta principal: Qual é a diferença de uso das bicicletas pelos **clientes casuais e anuais (membros)**?
- Perguntas específicas:
> - Qual é a média de duração da locação das bicicletas?
> - Quais são os dias da semana com a maior/menor quantidade de locações?
> - Qual é o total de clientes por dia, mês e ano?
> - Quais são os tipos de bicicleta mais alugados?
> - Quais são as estações mais utilizadas?
> - Qual é a localização geográfica das retiradas e devoluções?
> - Quais são os horários do dia com maiores locações e devoluções?

### Upload dos dados (.csv)
- Todos os arquivos (datasets) foram carregados para um volume dentro de um SQL Warehouse no Databricks (portfolio_citybikes)
- Posteriormente, foram criadas delta tables em lotes de 10 em 10 de maneira manual através da interface do Databricks (/Volumes/)
- A tabela com o modelo de esquema foi criada inicialmente a partir do arquivo "divvy_trips_2020_q_1.csv"
