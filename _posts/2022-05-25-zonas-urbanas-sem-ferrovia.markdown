---
layout: post
title:  "Onde falta metro/ferrovia na Área Metropolitana de Lisboa? (Parte 1 - Introdução)"
date:   2022-05-25 11:13:00 +0100
categories: lisboa mobilidade
---

A mobilidade na Área Metropolitana de Lisboa (AML) tem sido um tema em debate nos últimos anos. Apesar de às vezes o debate estar desnecessariamente incendiado, é positivo ver a preocupação de partidos políticos sobre temas como a redução da velocidade nas ruas de Lisboa, se a expansão do Metropolitano de Lisboa deve ser com uma linha circular ou em laço, ou a resistência da sociedade civil à remoção da ciclovia da Almirante Reis.

Apesar de ser necessário o debate político sobre estes temas, não devemos esquecer que estas decisões são também inerentemente técnicas e devem ser fundamentadas com dados. Nesta análise, o objectivo é encontrar na AML áreas de elevada densidade residencial e onde se demora muito tempo a pé até uma estação de metro/comboio.

# Porquê só comboio e metro? E os autocarros?
Não é por acaso que tantas cidades de média ou grande dimensão apostam em comboios, elétricos de superfície, ou metropolitano subterrâneo. Como se pode ver na página 14 do [Global Street Design Guide][gsdg], o transporte em metro ligeiro de superfície consegue transportar, no mesmo espaço, muitíssimo mais pessoas que o transporte feito em carros privados. A ferrovia pesada (comboios suburbanos e metro subterrâneo) tem capacidade ainda maior.

Quanto aos autocarros, podem ter a vantagem de um menor investimento inicial e de maior flexibilidade caso se queira mudar a rota. No entanto, dada a ausência de canais dedicados (faixas BUS e semáforos que fiquem verdes para um autocarro sempre que este se aproxime), especialmente fora do município de Lisboa, terão de se misturar com o trânsito geral. Nesse caso, o desempenho é bastante inferior ao de um canal ferroviário, como se pode ver também na página 14 do [Global Street Design Guide][gsdg].

Apesar destas vantagens do modo ferroviário dentro de áreas metropolitanas, não deixa de ser um modo que exije investimento considerável à cabeça. É, portanto, um tipo de transporte que habitualmente se usa apenas para zonas de densidade urbana elevada.

# Densidade populacional na AML
Olhemos então para a densidade residencial dentro da AML. Não podemos ter estações ferroviárias em cada quarteirão, pelo que faz sentido tê-las nas zonas onde antecipamos que haja procura elevada, ou onde antecipamos que venha a haver essa procura no futuro.

Tanto quanto sei não há, em Portugal, dados abertos sobre os percursos feitos pelas pessoas nas suas deslocações quotidianas. Também não conheço nenhuns dados sobre a densidade de postos de trabalho, que seria importante para esta análise.

No entanto, nos Censos de 2021, onde já estão disponíveis os dados provisórios, temos informação de número de residentes ao nível do quarteirão. Podemos analisar a densidade populacional de cada quarteirão a partir destes dados, e procurar zonas de elevada densidade que estejam longe de estações de metro e comboio.

Para calcular a densidade populacional segue-se este processo:
- Os dados provisórios dos Censos 2021 indicam, para cada quarteirão, quantas pessoas lá residem.
- Para cada quarteirão, os Censos também nos indicam a região geográfica que ocupa, permitindo assim calcular a área desse quarteirão em metros quadrados.
- Usando a população residente em cada quarteirão e a sua área, podemos calcular a densidade populacional de cada quarteirão.

O mapa que se segue mostra a densidade populacional num mapa 3D da AML. Quanto maior a altura de um quarteirão, maior a densidade populacional desse quarteirão.

{% include aml_population_density.html %}

Agora que já sabemos onde residem mais ou menos pessoas, podemos passar ao passo seguinte: incluir no mapa informação sobre ser fácil ou difícil usar modos ferroviários. Esse é o assunto da Parte 2.


[gsdg]: https://globaldesigningcities.org/wp-content/uploads/guides/global-street-design-guide.pdf
[metro2009]: https://pt.wikipedia.org/wiki/Metropolitano_de_Lisboa#Projetos_Anteriormente_Apresentados
[osm]: [https://www.openstreetmap.org/]
[ors]: [https://openrouteservice.org/]
[ciclovias.pt]: [https://www.ciclovias.pt/?lat=38.57706&lng=-9.04511&z=14.52900000000001&m=r&l=16]