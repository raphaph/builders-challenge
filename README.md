# Builders-challenge

Como linguagem utilizei python com modelo de com notebook jupiter pra separar cada conjunto de dados e seus tratamentos, são basicamentes 2/3 etapas apenas paras as fonte de dados, conforme indicadores solicitados.

Uso lib **pandas** para tratar os dataframes criados a partir dos dados extraídos, poderia usar também **Spark** ou **SQL** também no qual domino, porém o pandas da conta desse trabalho.

**dCalendar** - Criada para servir como nó principal das tabelas, e reunindo os relatórios em apenas um arquivo.

**COVID**
path: ETL/covid/_covid_extract_tranforms.ipynb
Notas
- De início preferi remover as linhas de 2 estados que as cidades vinham em branco, código ibge 12 e 27 dos estados, estavam na coluna de código das cidades. Não enxerguei outra forma de tratar essas informações.
- Criei 2 visões de acumulado, um dia a dia, e outro agrupando a coluna 'epidemiological_week', além de criar o rank de mortes por cidade.
- Observei que a base é pequena e tem apenas 2 estados, sendo AL um estado com bem pouca informação, para fins comparativo não é muito bom.

**MULTAS** 
path: ETL/multas/_multas_extract_tranforms.ipynb
Notas
- Fiz apenas um pequeno tratamento para junção da coluna mês e ano para padronizar com a dCalendar

Obs -> Por fim não utilizei no dashboard as tabelas com pósfixo '_grouped', demais tabelas foram suficiente.

---

Paths:
📂 dashboard-powerbi/builders-challenge.pbix
📂 ETL/covid/notebook e tabelas.csv
📂 ETL/multas/notebook e tabelas.csv
📂 ETL/dCalendar_notebook & tabela.csv

