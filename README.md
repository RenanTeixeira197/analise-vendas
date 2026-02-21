# analise-vendas

📊 Análise Exploratória de Vendas (2015–2018)
📌 Sobre o Projeto
Este projeto tem como objetivo realizar uma Análise Exploratória de Dados (EDA) em uma base de vendas contendo informações de pedidos, datas, regiões, categorias de produtos e segmentos de clientes.
A análise foi conduzida utilizando Python e Pandas, com foco em geração de métricas estratégicas para suporte à tomada de decisão.

🎯 Objetivos da Análise
Calcular métricas principais de desempenho (KPIs)


Identificar tendências temporais


Avaliar performance por região e estado


Analisar categorias e produtos mais rentáveis


Entender o comportamento por segmento de cliente


Detectar possíveis inconsistências nos dados



🛠 Tecnologias Utilizadas
Python


Pandas


NumPy


Matplotlib / Seaborn (para visualizações)


Jupyter Notebook



📈 Principais KPIs
Métrica
Valor
Receita Total
$2.261.536,79
Número de Pedidos
4.922
Ticket Médio
$459,48
Período Analisado
2015 – 2018


📊 Análise Temporal
Receita por Ano
Ano
Receita
2015
$479.856
2016
$459.436
2017
$600.192
2018
$722.052

📌 Observação:
 Após leve retração em 2016, houve crescimento consistente até 2018.

Receita por Mês (Sazonalidade)
Destaques:
🔝 Novembro: $350.161


🔝 Dezembro: $321.480


🔻 Fevereiro: $59.371


📌 Indicação clara de sazonalidade no último trimestre do ano.

🌎 Performance Geográfica
Receita por Região
Região
Receita
West
$710.219
East
$669.518
Central
$492.646
South
$389.151

A região Oeste lidera o faturamento.

Estados com Maior Receita
California — $446.306


New York — $306.361


Texas — $168.572


Washington — $135.206


Pennsylvania — $116.276



🛍 Performance por Produto
Receita por Categoria
Categoria
Receita
Technology
$827.455
Furniture
$728.658
Office Supplies
$705.422

A categoria Technology é responsável pela maior fatia do faturamento.

Top Produto por Receita
Canon imageCLASS 2200 Advanced Copier
 Receita acumulada: $61.599



Subcategorias com Maior Receita
Phones


Chairs


Storage


Tables



👥 Segmento de Clientes
Segmento
Receita
Consumer
$1.148.061
Corporate
$688.494
Home Office
$424.982

O segmento Consumer representa aproximadamente 51% da receita total.

🔎 Validação e Tratamento de Dados
Foi realizada conversão e validação das colunas de data:
df['Order Date'] = pd.to_datetime(df['Order Date'], dayfirst=True)
df['Ship Date'] = pd.to_datetime(df['Ship Date'], dayfirst=True)

dados_incoerentes = df[df['Ship Date'] < df['Order Date']]
Resultado:
 Nenhuma inconsistência encontrada após correção.

📌 Principais Insights Estratégicos
Crescimento consistente após 2016


Forte sazonalidade no último trimestre


Alta concentração de receita na Califórnia


Tecnologia é principal motor de receita


Segmento Consumer lidera faturamento



🚀 Possíveis Evoluções do Projeto
Implementação de Dashboard em Power BI ou Streamlit


Análise de lucratividade (Profit Margin)


Clusterização de clientes


Modelo preditivo de vendas


Deploy de dashboard em ambiente web



📎 Conclusão
A análise permitiu identificar padrões de crescimento, sazonalidade e concentração geográfica da receita, fornecendo base estratégica para decisões comerciais e expansão de mercado.


