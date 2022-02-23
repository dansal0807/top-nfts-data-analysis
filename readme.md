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

