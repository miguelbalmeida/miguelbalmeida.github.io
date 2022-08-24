---
layout: post
title:  "Onde falta metro/ferrovia na Área Metropolitana de Lisboa? (Parte 5 - Conclusão)"
date:   2022-05-25 11:13:00 +0100
categories: lisboa mobilidade
image: AML_distance_to_rail_stations_header_1.png
---

# Próximos passos
Há muito para onde ir após esta análise. Em primeiro lugar, há outras zonas da AML cujas análises ainda não publiquei, mas que estão em curso, incluindo:
- Lisboa Oeste
- Oeiras
- Almada
- Montijo
- Seixal

A análise pode ser também estendida a outras partes do país, nomeadamente a Área Metropolitana do Porto, ou Coimbra, que tem recentemente debatido o [encerramento da sua estação ferroviária mais central](https://www.publico.pt/2022/05/18/opiniao/opiniao/encerramento-estacao-central-coimbra-2006620).

Seria igualmente importante analisar o desempenho de outras partes do sistema de mobilidade da AML, em particular o desempenho dos autocarros. Ao contrário dos sistemas ferroviários aqui analisados, os autocarros são geralmente vulneráveis ao trânsito. Mesmo que existam carreiras de autocarro a servir certas zonas, isso não significa que esse serviço tenha a frequência, pontualidade e rapidez necessárias para ser competitivo com o uso do automóvel privado.

# Detalhes técnicos
Seria possível escolher à mão os bairros um a um para incluir nestas zonas, o que permitiria delimitar zonas mais densas ou com maior percentagem de população longe de estações. Optei ainda assim por usar freguesias porque:
- É mais simples de explicar qual a área sob análise.
- Permite mais facilmente a quem lê saber quais os órgãos políticos que governam essa área (as Juntas de Freguesia e Câmaras Municipais.correspondentes)
- É menos arbitrário.

Seria também possível corrigir, para as freguesias que incluem "bairros" sobre o rio Tejo, os valores da área respectiva. Optei por não o fazer pelas seguintes razões:
- Alguns bairros incluem grandes áreas sobre o rio mas também algumas áreas terrestres, e não é possível separar uma da outra nos dados dos Censos.
- O mesmo raciocínio justificaria outras correcções, como por exemplo retirar a zona do aeroporto de Lisboa da freguesia dos Olivais. Se fôssemos por aí, haveria um grande número de correcções algo arbitrárias a fazer.

Os dados provisórios dos Censos 2021 foram obtidos através do [site do INE](http://mapas.ine.pt/download/index2021.phtml).

Os tempos de deslocação a pé foram calculados usando o [Open Route Service][ors], que se baseia no [Open Street Map][osm]. O Open Route Service permite pedir direcções no seu site, mas rapidamente chegamos ao limite diário quando tentamos o número de caminhos necessários para esta análise. Assim, optei por colocar a correr no meu computador uma cópia do Open Route Service que eles próprios disponibilizam [no seu Github](https://github.com/GIScience/openrouteservice). Isto permite-me calcular tantos caminhos a pé quanto eu queira, limitado apenas pelo poder computacional do meu computador.

O Open Street Map também foi usado para determinar a posição de cada estação ferroviária. Seria possível usar alternativas como o Google Maps, e a sua API de direcções, mas preferi optar por dados e programas abertos que qualquer pessoa pode consultar e até corrigir. Além disso, a API do Google Maps é paga.

O tratamento de dados foi feito utilizando um computador pessoal e software Python. A maioria dos cálculos numéricos foram feitos com [geopandas](https://geopandas.org/en/stable/) e os mapas foram feitos usando [Kepler.gl](https://kepler.gl/), um software aberto de visualização de dados geográficos feito pela Uber.

O blogue é criado usando [Github Pages](https://pages.github.com/) e [Jekyll](https://jekyllrb.com/). O design gráfico é adaptado da excelente configuração [Millenial](https://jekyllthemes.io/theme/millennial) feita por Paul Le.

[gsdg]: https://globaldesigningcities.org/wp-content/uploads/guides/global-street-design-guide.pdf
[metro2009]: https://pt.wikipedia.org/wiki/Metropolitano_de_Lisboa#Projetos_Anteriormente_Apresentados
[osm]: [https://www.openstreetmap.org/]
[ors]: [https://openrouteservice.org/]
[ciclovias.pt]: [https://www.ciclovias.pt/?lat=38.57706&lng=-9.04511&z=14.52900000000001&m=r&l=16]