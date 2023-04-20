[PT-BR - english version below]
# Perguntas orientadoras da análise:

- Quais indicadores devo olhar para encontrar um possível sucesso com os dados que me foram dados?
- Existe alguma relação inerente a esses dados?
- Quais dados extrensícos ao dataset coletado devo considerar para não enviesar absolutamente minha análise?

Suas devidas respostas estão na conclusão do notebook e reproduzidas aqui:

# Premissas:
1. O market cap é o que entenderíamos pela receita total do projeto. No entanto, muitos indicadores (incluindo a coingecko), simplesmente multiplicam a quantidade de NFTs (total assets) pelo preço do NFT mais baixo (floor price), o que significa que não é exatamente confiável. O market cap é o melhor parâmetro para entender o crescimento do projeto a longo prazo e o seu sucesso, porém, como tudo em finanças, não é uma medida exata, existem diversos outros fatores que garantem o sucesso de um projeto.

2. Podemos considerar, por ser os top projetos NFTs, que eles deram sold out, ou seja, eles foram completamente vendidos. Por que isso é relevante? Quando um projeto tem todos seus NFTs vendidos, ele é considerado um bom projeto e o seu floor price se estabiliza, na maioria das vezes. Não é incomum um projeto estar completamente vendido.

3. Como busco identificar quais projetos se destacam de alguma maneira e quais indicadores a maior parte dos projetos possuem, as colunas que devem ser ressaltadas são: o floor price, market cap e owners (preço de "chão" (preço do NFT mais barato), receita do projeto e os proprietários).

# Conclusões:
1. É importante notar que como essa análise é dinâmica, muitas vezes os números indicados serão completamente diferentes por questões de flutuação de mercado. Nesse sentido, tentei fazer uma análise das relações de forma a priori, respaldadas pelos projetos principais da opensea de fevereiro, daqui a uma semana ou um mês ou um ano serão completamente diferentes.

2. Os dados acerca do floor price estão concentrados por volta de 0 e 5 ETH. O que nos indica lançamentos baixos, exceto por alguns outliers discrepantes.

3. A conclusão é que o Market Cap se mantém estável de um modo geral para a maior partes dos projetos tirando alguns Outliers acima de 20.000, ou ainda, podemos considerar que os Outliers se comprometem bastante acima do 3º Quartil (75%): 13587.1 ETH. Ainda mais quando se considera que a mediana é 2179 ETH, podemos entender que a maior parte dos projetos deve estar por volta desse valor.

4. Importante: Diante dos gráficos, conseguimos compreender que ainda existe uma boa dispersão acima de por volta de 3000 ETH de market cap. Os projetos acima disso são os que devem ter uma atenção interessante para um investidor.
 - Os proprietários do NFTs obedecem uma métrica muito mais concisa. O que isso nos indica?
 
O fato é que um proprietário pode ter muitos NFTs e não possuímos esse número somente com essa feature. No entanto, o que podemos inferir é que os projetos que possuem muitos proprietários:Estão completamente vendidos ou quase completamente.Esses NFTs têm um preço baixo ou o projeto tem muita fama. Os projetos que têm poucos proprietários ou têm um preço alto ou têm pouco sucesso.

5. A média de totais de NFTs (total assets) dos projetos é 7796. A maior parte dos projetos, no entanto se concentra em 9409 ~ 10.000 NFTs.

6. No dia 10/02, encontrei nenhum market cap maior que a multiplicação entre floor price e market cap.Portanto, o que indica é que essa coluna não é verídica. O interessante é notar que isso baliza o investidor por baixo, sabemos que a receita do projeto é, no mínimo, o market cap indicado no dataset.

7. Não necessariamente um projeto terá mais proprietários quando se tem mais ativos, visto que um projeto pode ter muitos ativos e poucos donos - o que indicaria, muito provavelmente, que os ativos estão em um preço baixo, mas com expectativa de lucro.

8. Se o projeto tem muitos ativos e muitos donos, é muito provável que o preço esteja razoalvemente equilibrado na proporção entre os dois. Essa relação é espelhada na coluna owners_ratio.

## Esses pontos foram colhidos através da observação dos gráficos e dos parâmetros estatísticos. Eles auxiliam algumas coisas em relação as perguntas iniciais:

<b> Primeiro pergunta </b>: Diante do que foi escolhido, e tomado como premissa, certamente o market cap é essencial. Percebemos também que o floor price é essencial para um investidor visto como a open sea e a coingecko (por consequência) o tomam como baliza mínima de valor. A quantidade de proprietários é essencial para compreendermos o quanto aquele projeto é atraente, no entanto, nada nos indica que quanto mais proprietários, mais valorizado é aquele projeto, para isso é preciso analisar em conjunto com o price floor e o market cap.

<b> Segunda pergunta </b>: Como demonstrei, o market cap é associado ao price floor e a quantidade total de NFTs em um projeto (total assets). Também é interessante notar o owner ratio, que nos mostra o quanto aquele projeto tem em termos de proporção de proprietários e ativos do projeto e como isso é significativo para saber o quão populoso é um projeto. A partir disso, podemos balizar também pela média de NFTs de um projeto. Acredito que isso é interessante de se comparar, se determinado projeto tá acima ou baixo da média em relação à quantidade de NFTs ofertados e relacionar isso com o owner ratio.

<b> Terceira Pergunta </b>: Isso é um toque mais pessoal que o dataset não fornece de maneira alguma. O que podemos inferir do dataset é quais projetos valem a pena se aprofundar quanto a essa questão. Para além de questões puramente matemática e financeiras, a questão gira em torno do quanto aquele projeto é sustentável de um ponto de vista tecnológico e de constituição de comunidade.

------------------------------------------------------------
[EN] 
# Analysis guiding questions:

- What indicators should I look at to find possible success with the given data?
- Is there any inherent relationship among these data?
- What external data should I consider to avoid biasing my analysis?
- The answers to these questions are in the conclusion of the notebook and reproduced here:

# Premisses:

1. The market cap is what we would understand as the total revenue of the project. However, many indicators (including coingecko) simply multiply the number of NFTs (total assets) by the price of the lowest priced NFT (floor price), which means it is not exactly reliable. The market cap is the best parameter to understand the long-term growth and success of a project, but like everything in finance, it is not an exact measure, and there are various other factors that ensure the success of a project.

2. We can consider that since these are top NFT projects, they have sold out, meaning all their NFTs have been sold. Why is this relevant? When a project has all its NFTs sold, it is considered a good project and its floor price stabilizes, most of the time. It is not uncommon for a project to be completely sold out.

3. As I seek to identify which projects stand out in some way and what indicators most projects have, the columns that should be highlighted are: floor price, market cap, and owners (lowest NFT price, project revenue, and owners).

# Conclusions:

1. It is important to note that since this analysis is dynamic, the numbers indicated will often be completely different due to market fluctuations. In this sense, I tried to make an analysis of the relationships in a priori manner, based on the main projects on opensea in February, but in a week, a month, or a year, they will be completely different.

2. The data on floor price is concentrated around 0 and 5 ETH, indicating low launch prices, except for some discrepant outliers.

3. The conclusion is that the Market Cap remains stable in general for most projects, except for some outliers above 20,000, or we can consider that the outliers are considerably above the 3rd quartile (75%): 13587.1 ETH. Especially when considering that the median is 2179 ETH, we can understand that most projects are around that value.

4. Important: From the graphs, we can understand that there is still a significant dispersion above around 3000 ETH of market cap. Projects above this value should be of interesting attention to an investor.

The owners of the NFTs follow a much more concise metric. What does this indicate?
The fact is that an owner can have many NFTs, and we do not have that number only with this feature. However, what we can infer is that projects that have many owners: are completely sold out or almost completely sold out. These NFTs have a low price or the project is very famous. Projects that have few owners either have a high price or have little success.

5. The average total NFTs (total assets) of projects is 7796. However, most projects are concentrated in 9409 to 10,000 NFTs.

6. On February 10th, I found no market cap higher than the multiplication of floor price and market cap. Therefore, this column is not accurate. Interestingly, this sets a lower benchmark for investors, as we know that the project revenue is at least the market cap indicated in the dataset.

7. t is not necessarily the case that a project will have more owners when it has more assets, as a project can have many assets and few owners, which would likely indicate that the assets are priced low but with profit expectations.

8. If a project has many assets and many owners, it is very likely that the project is completely sold out or nearly sold out, indicating high demand and popularity.

## Answers to the initial questions:

1. To avoid bias in the analysis, it is important to consider external data such as market trends, project news, and community sentiment. Market fluctuations can significantly impact the numbers and rankings of NFT projects, so it's important to keep the dynamic nature of the NFT market in mind when interpreting the data.

2. In conclusion, the analysis suggests that floor price, market cap, and owners are key indicators to consider when assessing the success of NFT projects. Projects with low launch prices, stable market caps, and either many owners or high asset prices tend to stand out. However, it's important to consider external factors and keep in mind the dynamic nature of the NFT market when interpreting the data. Additionally, the dataset used for analysis may not be completely accurate, and further research and analysis may be needed to make informed investment decisions.

