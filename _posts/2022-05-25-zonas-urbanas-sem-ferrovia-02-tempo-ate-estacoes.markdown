---
layout: post
title:  "Onde falta metro/ferrovia na Área Metropolitana de Lisboa? (Parte 2 - Tempo a pé até uma estação)"
date:   2022-05-25 14:13:00 +0100
categories: lisboa mobilidade
---

Na [Parte 1]({% post_url 2022-05-25-zonas-urbanas-sem-ferrovia %}) olhámos para um mapa com a densidade populacional da AML. Agora falta encontrar quais as zonas onde o metro e o comboio não sejam opção prática. Para isso podemos calcular o tempo a pé até à estação ferroviária mais próxima.

# Tempo a pé a a estações ferroviárias
Para esta análise olhei para as seguintes linhas ferroviárias, num total de 155 estações:
- As quatro linhas do Metropolitano de Lisboa.
- As quatro linhas suburbanas da CP dentro da AML: linha do Sado (que liga o Barreiro a Praias do Sado, passando por Setúbal), linha da Azambuja, linha de Sintra e linha de Cascais.
- Acrescentei ainda as estações da linha do Oeste da CP que estão dentro da AML, embora não sejam serviços suburbanos.
- A linha do Sul, operada pela Fertagus, que passa na Ponte 25 de Abril e liga o município de Lisboa a Setúbal, num percurso diferente da linha do Sado.
- O Metro Sul do Tejo.

Pegando no mapa da Parte 1, podemos agora adicionar informação sobre a proximidade a uma estação ferroviária. O processo é o seguinte:
- O [Open Street Map](https://www.openstreetmap.org/) diz-nos onde se localiza cada estação ferroviária.
- Para cada um dos 25915 quarteirões dos Censos, que estão no mapa da Parte 1, calculei o centróide, ou seja, o ponto central desse quarteirão.
- Finalmente, usei o [Open Route Service](https://openrouteservice.org/) para calcular o tempo necessário para ir a pé entre todos os centróides e todas as estações ferroviárias. Guardei, para cada quarteirão, a estação mais próxima e o tempo que se leva a pé até ela.

Este último passo não é diferente do que o leitor provavelmente já fez usando aplicações como o Google Maps ou o Apple Maps, mas é automatizado. Isso permite o cálculo de tempos de deslocação a pé entre os 25915 quarteirões da AML e as 155 estações ferroviárias que mencionei em cerca de meia hora num computador moderno.

No mapa abaixo, as tonalidades de verde representam o tempo de deslocação a pé até à estação ferroviária mais próxima. Há cinco tonalidades de verde para representar os seguintes intervalos:
- 0 a 5 minutos a pé (verde escuro)
- 5 a 10 minutos a pé
- 10 a 15 minutos a pé
- 15 a 20 minutos a pé
- mais do que 20 minutos a pé (branco)

{% include aml_population_density_with_distance_to_rail_stations.html %}

Rodando e fazendo "zoom" conseguimos ver no mapa várias zonas densamente povoadas onde a maioria dos quarteirões estão a mais de 20 minutos a pé de estações ferroviárias. Nas páginas que se seguem olharemos para algumas delas em mais detalhe, começando com a zona Oeste de Odiveias, que é o assunto da [Parte 3]({% post_url 2022-05-25-zonas-urbanas-sem-ferrovia-03-odivelas-oeste %}). A [Parte 4]({% post_url 2022-05-25-zonas-urbanas-sem-ferrovia-04-odivelas-leste %}) analisa a zona Leste de Odiveias em conjunto com o Sul de Loures.

[gsdg]: https://globaldesigningcities.org/wp-content/uploads/guides/global-street-design-guide.pdf
[metro2009]: https://pt.wikipedia.org/wiki/Metropolitano_de_Lisboa#Projetos_Anteriormente_Apresentados
[ciclovias.pt]: [https://www.ciclovias.pt/?lat=38.57706&lng=-9.04511&z=14.52900000000001&m=r&l=16]