# builders-challenge

Escolhi a lib **pandas** por ter mais experiência, porém poderia ter usado **Spark** também no qual domino.

Escolhi o modelo de notebook do jupiter pra separar cada conjunto de dados e seus tratamentos, são basicamentes 3 etapas pra cada fonte de dados, conforme indicadores solicitados.

**dCalendar** - Criada para servir como nó principal das tabelas, e reunindo os relatórios em apenas um arquivo.

*COVID* - Notas
- De início preferi remover as linhas de 2 estados que as cidades vinham em branco, código ibge 12 e 27 dos estados, estavam na coluna de código das cidades. Não enxerguei outra forma de tratar essas informações.
- Criei 2 visões de acumulado, um dia a dia, e outro agrupando a coluna 'epidemiological_week', além de criar o rank de mortes por cidade.
- Observei que a base é pequena e tem apenas 2 estados, sendo AL um estado com bem pouca informação, para fins comparativo não é muito bom.

*MULTAS* - Notas
- Fiz apenas um pequeno tratamento para junção da coluna mês e ano para padronizar com a dCalendar