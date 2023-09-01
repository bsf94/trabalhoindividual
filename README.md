# Projeto individual: Análise da relação entre liberdade econômica e o crescimento do PIB no Brasil.
- **OBJETIVO:** O objetivo deste projeto é analisar a relação entre o crescimento do PIB no Brasil e o nível de liberdade econômica, conforme medido pelo Índice Economic Freedom of the World (EFW).  
- **RELEVÂNCIA:** Através dessa análise, espera-se identificarse se há relação entre o nível de liberdade econômica no país e variações no crescimento do PIB. Essas informações podem ser úteis para o entendimento de fatores relacionados à políticas públicas que visem melhorar a liberdade econômica e impulsionar o crescimento econômico sustentável no Brasil, caso esteja relação seja encontrada.
- **CONTEXTO:** Este projeto tem como foco o Brasil e busca analisar a relação entre o crescimento do PIB e a liberdade econômica no país. Para isso, serão utilizados dados entre o período de 2000 a 2020. Esse intervalo de tempo permitirá uma análise ampla e aprofundada das tendências e correlações ao longo das últimas duas décadas. 
- **LIMITAÇÕES:** Este projeto apresenta algumas limitações importantes a serem consideradas. Primeiramente, é fundamental reconhecer que correlação não implica causalidade. Mesmo que seja possível identificar correlações entre os indicadores de liberdade econômica e o crescimento do PIB, estabelecer uma relação causal é mais complexo. A liberdade econômica é apenas um dos muitos fatores que influenciam o crescimento do PIB, e há muitas outras variáveis que impactam o PIB de um país, como estabilidade política e social, investimento em infrastrutura, desenvolvimento de capital humano, nível de educação da população, condições macroeconômicas nacionais e globais, fatores demográficos, etc. Esse projeto irá aborar apenas um aspecto geral - o nível de liberdade econômica - e cinco subcomponentes: tamanho do governo, sistema jurídico e direito de propriedade, sound money, liberdade de comércio internacional e regulamentos.


# O que é liberdade econômica?
"The key ingredients of economic freedom are personal choice, voluntary exchange, freedom to compete, and protection of persons and property. When economic freedom is present, the choices of individuals will decide what and how goods and services are produced. [...] However, economic freedom also requires governments to refrain from many activities. They must refrain from actions that interfere with personal choice, voluntary exchange, and the freedom to enter and compete in labor and product markets." (GWARTNEY; LAWSON, 2003, p. 406)

- **Porque o EFW?** Neste projeto, o uso do Índice EFW se justifica devido à sua relevância como uma medida abrangente e amplamente reconhecida para avaliar o nível de liberdade econômica de um país. O índice é baseado em uma estrutura teórica sólida e abrange diversas dimensões, como o tamanho do governo, a eficiência judicial, a liberdade de comércio, sound money e a proteção dos direitos de propriedade. Ao utilizar esse índice, é possível quantificar e comparar o grau de liberdade econômica entre diferentes países, bem como identificar quais subcomponentes têm maior impacto no nível geral de liberdade econômica. A primeira publicação do relatório Economic Freedom of the World foi publicada em 1996, resultado de uma série de conferências realizadas entre 1986 e 1994, com o propósito de desenvolver uma definição clara e quantitativa de liberdade econômica. O índice considera cinco áreas principais, que possuem sub-componentes, que por sua vez também podem apresentar subcomponentes. No total, o índice considera 44 variáveis. Nesse trabalho, iremos trabalhar apenas com o nível geral de liberdade econômica e os 5 grandes componentes do índice, pois o número de subcomponentes variou nas últimas duas décadas e não seria possível obter dados consistentes para todas as variáveis. 
- **Componentes do EFW:** O score geral do EFW é resultado da média dos cinco componentes abaixo, que serão utilizados nesse trabalho.

|   | Componentes | 
|---|----------|
| 1 | Government Size (Tamanho do governo)        | 
| 2 | Legal System & Property Rights (Sistema jurídico e direitos de propriedade)        | 
| 3 | Sound money (Moeda sólida)        |                              |
| 4 | Freedom to trade internationally (Liberdade de comércio internacional)        |
| 5 | Regulation (Regulamentos)        | 


# Coleta de dados

- Índice EFW: Os dados estão disponíveis [no site do Instituto Frasier](https://www.fraserinstitute.org/economic-freedom/dataset?geozone=world&page=dataset&min-year=2&max-year=0&filter=0), responsável pelo lançamento de um relatório anual que mede o nível de liberdade econômica em diversos países do mundo. 
- PIB, Unemployment, PolStab: Os dados estão disponíveis [no site do World Bank](https://data.worldbank.org/).
- CPI: Os dados estão disponível [no site transparency.org](https://www.transparency.org/en/cpi/2021)
  
# Dicionário de dados

| Variável | Descrição                                              | Tipo | Observações                                                                                                          |
|---------------|----------------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------|
| GDP           | Gross Domestic Product (GDP)                             | Numeric   | GDP (PIB) mede o valor total de bens e serviços produzidos dentro de um país durante um período. |
| EFW           | Economic Freedom of the World Index (EFW)                             | Numeric   | EFW is a measure of the degree of economic freedom within a country.                                             |
| GovSize       | Government Size                                     | Numeric   | Mede o grau de intervenção governamental na economia, incluindo gastos governamentais, tributação e o tamanho das empresas estatais.                                 |
| LegalSystem   | Legal System and Property Rights                                       | Numeric   | Medee a eficiência  do estado de direito, a independência do judiciário, a segurança dos direitos de propriedade e a eficácia da execução de contratos.                       |
| TradeFreedom  | Freedom to trade Internationally                                     | Numeric   | Refere-se ao grau de abertura e liberdade que um país tem para realizar o comércio internacional, incluindo a ausência de tarifas, barreiras e restrições nas importações e exportações, bem como a liberdade de participar de trocas internacionais sem interferência governamental excessiva.
| SoundMoney    | Sound Money                                        | Numeric   | Refere-se à estabilidade e confiabilidade do sistema monetário de um país, incluindo baixas taxas de inflação, ausência de controles de preços e a capacidade dos indivíduos de usar e manter sua forma preferida de dinheiro sem restrições governamentais.
| Regulation    | Regulation                                         | Numeric   | Refere-se ao grau de intervenção e regulação governamental na economia, incluindo regulamentações comerciais, restrições no mercado de trabalho e burocracia.                       |
| CPI    | Corruption Perception Index                                         | Numeric   | Refere-se ao de corrupção no país, em uma escala de 1-100.                       |
| PolStab    | Political Stability                                         | Numeric   | Refere-se a estabilidade política no país.                       |
| Unemployment    | Desemprego                                         | Numeric   | Refere-se ao percentual da força de trabalho que está desempregada.                       |
| PIB/capita    | PIB per capita                                         | Numeric   | Refere-se ao produto interno bruto per capita.                       |

# REFERÊNCIAS

GWARTNEY, J.; LAWSON, R. The concept and measurement of economic freedom. European Journal of Political Economy, v. 19, n. 3, p. 405-430, 2003. Disponível em https://doi.org/10.1016/S0176-2680(03)00007-7 Acesso em: 18 maio 2023.

