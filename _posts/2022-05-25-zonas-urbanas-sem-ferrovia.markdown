---
layout: post
title:  "Onde falta metro/ferrovia na Área Metropolitana de Lisboa? (Parte 1 - Introdução)"
date:   2022-05-25 15:13:00 +0100
categories: lisboa mobilidade
---

![Imagem]({{ site.url }}/assets/img/AML_distance_to_rail_stations_header_2.png)

A mobilidade na Área Metropolitana de Lisboa (AML) tem sido um tema em debate nos últimos anos. Apesar de às vezes o debate estar desnecessariamente incendiado, é positivo ver a preocupação de partidos políticos sobre temas como a [redução da velocidade nas ruas de Lisboa](https://cnnportugal.iol.pt/videos/reducao-dos-limites-de-velocidade-em-lisboa-motiva-debate-aceso-na-camara/628e85480cf2ea4f0a4c6b0c), se a expansão do Metropolitano de Lisboa deve ser [com uma linha circular ou em laço](https://lisboaparapessoas.pt/2021/11/19/metro-lisboa-expansao-linha-circular-camara-governo-pcp-moedas/?doing_wp_cron=1651066237.3754520416259765625000), ou a [resistência da sociedade civil à remoção da ciclovia da Almirante Reis](https://expresso.pt/sociedade/2021-11-30-Mais-de-2500-lisboetas-levam-peticao-a-Assembleia-Municipal-para-travar-fim-da-ciclovia-da-Almirante-Reis-22a9ff45).

Apesar de ser necessário o debate político sobre estes temas, não devemos esquecer que estas decisões são também altamente técnicas e devem ser fundamentadas com dados. Nesta análise, o objectivo é ajudar a informar o debate sobre mobilidade na AML, procurando áreas de elevada densidade residencial e onde se demora muito tempo a pé até uma estação de metro/comboio.

# Porquê só comboio e metro?
Não é por acaso que tantas cidades de média ou grande dimensão apostam em comboios, elétricos de superfície, ou metropolitano subterrâneo. A tabela abaixo apresenta o número máximo de pessoas que passam por hora numa faixa de 3 metros de largura, usando números retirados da página 14 do [Global Street Design Guide][gsdg]. 

| Tipo de faixa (largura: 3 metros) | Pessoas por hora |
| --- | --- |
| Automóveis privados | 600-1.600 |
| Automóveis privados e autocarros frequentes | 1.000-2.800 |
| Ciclovia bidirecional | 6.500-7.500 |
| Autocarros em Faixas BUS | 4.000-8.000 |
| Pessoas a pé no passeio | 8.000-9.000 |
| Metro de superfície ou *bus rapid transit* | 10.000-25.000 |

Alguns destes números podem não ser intuitivos - por exemplo, um passeio com 3 metros de largura permite a passagem de 8000 a 9000 pessoas por hora, o que é muito superior a uma faixa apenas usada por automóveis privados (600-1600 pessoas por hora). A nossa intuição diz-nos que quanto mais rápido andamos, mais pessoas podem passar por hora, mas um carro ocupa um espaço muito maior que uma pessoa a pé. Ou seja, as pessoas a andar a pé andam mais devagar, mas podem andar muito mais próximas umas das outras.

É claro que em certas circunstâncias se justifica a menor capacidade do transporte em carro privado, por exemplo na rede de estradas nacionais e de auto-estradas. Não faz nenhum sentido pensar em substituir uma auto-estrada por passeios, porque nunca teremos 8000-9000 pessoas por hora interessadas em fazer Lisboa-Porto pela A1 a pé. No entanto, em meio urbano, a densidade de pessoas é maior e as velocidades médias de um automóvel são bastante mais baixas devido a cruzamentos, passadeiras, trânsito, etc. Nesse sentido, um passeio no centro de uma cidade frequentemente move mais pessoas que uma faixa para carros.

Segundo esta tabela, o transporte em metro ligeiro de superfície consegue transportar, no mesmo espaço, cerca de 10 vezes mais pessoas por hora que o transporte feito em carros privados.

## Exemplos da AML
Pegando num exemplo da própria AML, a capacidade da linha de Sintra é pelo menos de 16000 pessoas por hora. Isto porque cada comboio da linha de Sintra tem [capacidade para 1600 passageiros](https://sintranoticias.pt/2020/04/30/comboios-na-linha-de-sintra-a-circular-a-160-da-capacidade-maxima-permitida/), e à hora de ponta chegam a circular 10 comboios por hora nessa linha, isto num só sentido (basta consultar o [site da CP](https://www.cp.pt/passageiros/pt)). Para se mover o mesmo número de pessoas usando automóveis privados seria preciso um IC19 com 10 a 27 faixas de largura... para cada lado!

Um outro exemplo são os comboios do metropolitano de Lisboa, onde cada comboio tem uma capacidade de cerca de 1070 pessoas, segundo [este artigo da Wikipedia](https://pt.wikipedia.org/wiki/Material_circulante_do_Metropolitano_de_Lisboa#ML99) - assumindo 4 carruagens não motoras e 2 carruagens motoras por comboio - e chegam a passar a cada 4 minutos e 35 segundos na linha Azul, segundo a [página do próprio Metropolitano de Lisboa](https://www.metrolisboa.pt/viajar/horarios-e-frequencias/). Isto dá uma capacidade de cerca de 14000 pessoas por hora.

## E os autocarros?
Quanto aos autocarros, podem ter a vantagem de um menor investimento inicial e de maior flexibilidade caso se queira mudar a rota. No entanto, dada a ausência de canais dedicados (faixas BUS e semáforos que fiquem verdes para um autocarro sempre que este se aproxime), especialmente fora do município de Lisboa, terão de se misturar com o trânsito geral. Nesse caso, permitem sensivelmente duplicar o número de pessoas movidas por hora em relação a apenas carros (para 1000-2800), o que é bastante menos que multiplicá-lo por 10 ou mais como se consegue com canais ferroviários.

Apesar destas vantagens do modo ferroviário dentro de áreas metropolitanas, não deixa de ser um modo que exige investimento elevado à cabeça, especialmente se for subterrâneo, e cujo traçado é difícil de mudar. É, portanto, importante decidir bem por onde ele deve passar, para que o investimento seja justificado.

# Densidade populacional na AML
Olhemos então para a densidade populacional (ou seja, residencial) dentro da AML. Não podemos ter estações ferroviárias em cada quarteirão, pelo que faz sentido tê-las nas zonas onde haja procura elevada, ou onde se antecipa que haja essa procura no futuro.

Porquê densidade *populacional*? Os locais de trabalho e de estudo também geram viagens, certo? Certíssimo. A escolha de usar a densidade populacional é apenas por pragmatismo. 
Tanto quanto sei não há, em Portugal, dados abertos sobre os percursos feitos pelas pessoas nas suas deslocações quotidianas. Também não conheço nenhuns dados sobre a densidade de postos de trabalho, que seria importante para esta análise.

No entanto, nos Censos de 2021, onde já estão disponíveis [os dados provisórios](http://mapas.ine.pt/download/index2021.phtml), temos informação de número de residentes ao nível do quarteirão. Podemos analisar a densidade populacional de cada quarteirão a partir destes dados, e procurar zonas de elevada densidade que estejam longe de estações de metro e comboio.

Para calcular a densidade populacional segue-se este processo:
- Os dados provisórios dos Censos 2021 indicam, para cada quarteirão, quantas pessoas lá residem.
- Para cada um dos 25915 quarteirões da AML, os Censos também nos indicam a zona do mapa que ocupam, permitindo assim calcular a área de cada quarteirão em metros quadrados.
- Usando a população residente em cada quarteirão e a sua área, podemos calcular a densidade populacional de cada quarteirão.

O mapa que se segue mostra a densidade populacional num mapa 3D da AML. Quanto maior a altura de um quarteirão, maior a densidade populacional desse quarteirão. Pode fazer *zoom* com a roda do rato, clicar com o botão esquerdo para mover o mapa, ou com o botão direito para o rodar. Se passar o ponteiro do rato por cima de um quarteirão verá informações detalhadas sobre esse quarteirão - são os dados dos Censos.

{% include aml_population_density.html %}

Sabendo onde residem mais ou menos pessoas, podemos passar ao passo seguinte: incluir no mapa informação sobre ser fácil ou difícil usar modos ferroviários. Esse é o assunto da [Parte 2]({% post_url 2022-05-25-zonas-urbanas-sem-ferrovia-02-tempo-ate-estacoes %}).


[gsdg]: https://globaldesigningcities.org/wp-content/uploads/guides/global-street-design-guide.pdf
[metro2009]: https://pt.wikipedia.org/wiki/Metropolitano_de_Lisboa#Projetos_Anteriormente_Apresentados
[osm]: [https://www.openstreetmap.org/]
[ors]: [https://openrouteservice.org/]
[ciclovias.pt]: [https://www.ciclovias.pt/?lat=38.57706&lng=-9.04511&z=14.52900000000001&m=r&l=16]