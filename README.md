# Analise_de_Dados---Portal-da-transp-2025
Análise exploratória de dados públicos do Portal da Transparência sobre viagens a serviço de servidores públicos federais em 2025

##Etapas da Análise

###Leitura e limpeza dos dados

Carregamento do CSV com encoding Windows-1252
Tratamento de valores nulos na coluna Cargo
Conversão de colunas de texto para formato de data


###Criação de métricas

Despesas = Diárias + Passagens + Outros gastos
Dias de viagem = Data de fim − Data de início


###Consolidação por cargo

Agrupamento com groupby calculando: despesa média, duração média, despesas totais, destino mais frequente e número de viagens
Filtro de relevância: apenas cargos com mais de 1% do total de viagens


###Visualizações

Gráfico de barras horizontais: viagens por cargo público
Scatter plot: relação entre dias de viagem e despesas


###Identificação de outliers

Filtro de viagens com despesas acima de R$ 175.000


###União de tabelas

Cruzamento da tabela de Viagens com a tabela de Passagens via merge


##Principais Conclusões

-Os cargos mais operacionais e técnicos concentram o maior volume de viagens
-Existe correlação positiva entre dias de viagem e despesas, com dispersão relevante — outros fatores também influenciam o custo
-Foram identificadas viagens com gastos acima de R$ 175.000 (missões especiais, viagens internacionais ou inconsistências no registro)
-Uma parcela dos registros não possui cargo identificado (sigilo), o que aponta para lacunas no preenchimento dos dados pelo governo


##Fonte

[Portal da tranparência](https://portaldatransparencia.gov.br/viagens?ano=2025)

