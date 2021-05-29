<p align="center">
  <img src="https://15croum5v52u4nrv7goeotkw-wpengine.netdna-ssl.com/wp-content/uploads/2019/10/fourkites-datascience.jpg" width = 70%>
</p>


# Projeto: Ocorrências de Tráfego e o Impacto na Saúde Pública
---
Este repositório apresenta a o projeto desenvolvido para o Módulo 01 do Segundo Bootcamp de Ciência de Dados da Alura. Serão feitas análises em cima dos dados obtidos na fonte de dados abertos do DATASUS pelo serviço TABNET. Será realizada uma análise exploratória dos dados obtidos com uma explanação. Posteriormente, serão elaboradas hipóteses a serem confirmadas ou refutadas com a utilização de visualização de dados e conceitos de estatística.

# Dos Dados
---
Os dados trabalhados neste projeto são oriundos da fonte de dados abertos <a href="http://www2.datasus.gov.br/DATASUS/index.php?area=0202&id=11633&VObj=http://tabnet.datasus.gov.br/cgi/deftohtm.exe?sih/cnv/qi">DATASUS</a>, com a utilização do serviço TABNET. Foram selecionados os dados consolidados de todas as unidades da federação de Autorizações de Internações Hospitalares (AIH) separados por local de internação a partir do ano de 2008.

Como linha e coluna do dataset a ser gerado pelo TABNET, foram selecionadas "Unidade da Federação" e "Ano/mês processamento". O objetivo dessa seleção era prover uma série temporal de dados que possibilitasse separar as diversas regiões do país, com o intuito de se avaliar a influência destas nos dados analisados. Foi selecionado como conteúdo o "Valor total" filtrado pelo caráter de atendimento "Outros tipos de acidente de trânsito".

Um segundo dataset semelhante ao utilizado no módulo 01 foi utilizado com o intuito de se obter correlações com o novo dado obtido. Isto posto, como linha e colunas foram selecionadas "Unidade da Federação" e "Ano/mês processamento", respectivamente. Foi selecionado "Valor total" para o conteúdo sem qualquer outro tipo de filtro.

# Do Objetivo
---
Durante os estudos do módulo 01 especificado, surgiu a suspeita de que o movimento pendular de tráfego causado pelos períodos de festas e férias escolares aumentaria o gasto com saúde das unidades da federação. Fato este, causado em decorrência do aumento de ocorrências de tráfego nas estradas, além da imprudência e abuso de alcool por parte dos condutores no período. 

Este projeto tem o objetivo de visualizar a influência de gastos oriundos do tráfego de veículos em relação ao total gasto com saúde pública pela federação. Desta forma, seria evidênciado que não são apenas doenças e crises sanitárias que influenciam a evolução dos dados, sendo o tráfego um grande fator de gastos para a federação e tendo as campanhas de conscientização dos condutores como principal ferramenta para preservação da vida.

# Da Metodologia Utilizada
---
Precedendo as análises dos dados, foi necessária um pré-processamento das bases de dados, realizando cortes temporais e preenchimento de pequenos lapsos com interpolação linear. Foram criadas tabelas e gráficos de proporcionalidade e correlação com linhas de tendências para a avalização da influência de uma base na outra. 

# Resultados
---
* De 17 estados analisados, em 10 estados o gasto total com saúde pública aumenta com o gasto em acidentes.
* De 17 estados analisados, em 7 estados essa proporção é a inversa do item anterior.
* Os gastos com acidentes são muito menores que o gasto total com saúde pública.

# Conclusões
---
Os gastos em saúde pública oriundos de acidentes de tráfego não são significativos para os gastos totais com saúde pública. Uma segunda hipótese levantada durante a visualização dos gráficos de gastos com saúde pública devido a acidentes, é que os estados podem subnotificar estes gastos. No caso de um estado não classificar um gasto, automaticamente implica em adicioná-lo ao total e indicando ele como não sendo devido a um acidente de tráfego. Essa falta de classificação repetida por meses, pode impactar diretamente as análises.
