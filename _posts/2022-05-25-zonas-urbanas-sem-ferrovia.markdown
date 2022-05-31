---
layout: post
title:  "Onde falta metro/ferrovia na Área Metropolitana de Lisboa? (Parte 1 - Introdução)"
date:   2022-05-25 11:13:00 +0100
categories: lisboa mobilidade
---

# Porquê ferrovia?
Página 14 do [Global Street Design Guide][gsdg].

# A situação na AML

## Densidade populacional na AML
Em primeiro lugar, importa saber onde mora mais gente. Não podemos ter estações ferroviárias à porta de toda a gente, pelo que faz sentido ter ferrovia a passar apenas nas zonas mais densamente povoadas.

Para calcular a densidade populacional podemos usar os dados dos Censos:
- Os dados provisórios dos Censos 2021 indicam, para cada quarteirão, quantas pessoas lá residem.
- Para cada quarteirão, os Censos também nos indicam a região geográfica que ocupa, permitindo assim calcular a área desse quarteirão em metros quadrados.
- Usando a população residente em cada quarteirão e a sua área, podemos calcular a densidade populacional de cada quarteirão.

O mapa que se segue mostra a densidade populacional num mapa 3D da AML. Quanto maior a altura de um quarteirão, maior a densidade populacional desse quarteirão.

{% include aml_population_density.html %}

## Distância a estações ferroviárias
Tendo um mapa que mostra a densidade populacional da AML, podemos agora colori-lo conforme a distância de cada quarteirão a uma estação ferroviária.

Para esta análise olhei para as seguintes linhas ferroviárias, que totalizam um total de 156 estações:
- As quatro linhas do Metropolitano de Lisboa.
- As quatro linhas da CP dentro da AML: linha do Sado (que liga o Barreiro a Praias do Sado, passando por Setúbal), linha da Azambuja, linha de Sintra e linha de Cascais.
- Acrescentei ainda as estações da linha do Oeste da CP que estão dentro da AML, embora não sejam serviços urbanos.
- A linha do Sul, operada pela Fertagus, que passa na Ponte 25 de Abril e liga o município de Lisboa a Setúbal.
- O Metro Sul do Tejo.

O processo é o seguinte:
- O [Open Street Map][osm] diz-nos onde se localiza cada estação ferroviária.
- Para cada quarteirão dos Censos, calculei o centróide, ou seja, o ponto central desse quarteirão.
- Finalmente, usei o [Open Route Service][ors] para calcular as distâncias a pé entre todos os centróides e todas as estações ferroviárias. Guardei, para cada quarteirão, a estação mais próxima e o tempo que se leva a pé até ela.

No mapa da Figura 1, as tonalidades de verde representam a proximidade à estação ferroviária mais próxima. Há cinco tonalidades de verde para representar os seguintes intervalos:
- 0 a 5 minutos a pé (verde escuro)
- 5 a 10 minutos a pé
- 10 a 15 minutos a pé
- 15 a 20 minutos a pé
- mais do que 20 minutos a pé (branco)

{% include aml_population_density_with_distance_to_rail_stations.html %}

Rodando e fazendo "zoom" conseguimos ver no mapa várias zonas densamente povoadas onde todos os quarteirões estão a mais de 20 minutos a pé de estações ferroviárias. Olhemos para algumas delas em mais detalhe.

# Zonas sem ferrovia

## Odivelas Oeste
{% include map_odivelas_oeste.html %}

A zona sob análise está assinalada no mapa acima a azul. Inclui as seguintes freguesias:
- Município de Odivelas: Odivelas (freguesia); UF Pontinha e Famões; UF Ramada e Caneças. (UF = União de Freguesias, criadas aquando da reorganização administrativa de 2012)
- Município da Amadora: Encosta do Sol; Mina de Água.
- Município de Sintra: Casal de Cambra.

Esta zona tem:
- Área: 36.97 km2
- População residente: 212680
-- Dos quais 125547 (59%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 5753 pessoas por km2

Uma densidade populacional de 5753 pessoas por km2 é bastante elevada. Para termo de comparação, o município de Lisboa tem 24 freguesias, 13 das quais têm densidade populacional menor que 5753 pessoas por km2. Apenas 11 freguesias de Lisboa têm densidade populacional maior que este valor.

Partes desta zona estão relativamente perto de estações do Metro de Lisboa, nomeadamente da linha Amarela (a leste) e da linha Azul (a sul). Mas é inegável que a maioria da população desta zona não usará o metro regularmente, mesmo que trabalhe ou estude perto de uma estação de metro, dado que as estações estão demasiado longe da sua residência.

Não é portanto um acaso que o [plano de expansão do Metro de Lisboa de 2009][metro2009] incluísse expansões a servir esta zona, com prolongamento da linha Amarela.

## Odivelas Leste e Sul de Loures
{% include map_odivelas_leste_e_loures.html %}

Esta zona inclui as seguintes freguesias:
- Município de Odivelas: UF Póvoa de Santo Adrião e Olival Basto.
- Município de Loures: UF Moscavide e Portela; UF Sacavém e Prior Velho; UF Santa Iria de Azóia, São João da Talha e Bobadela; UF Camarate, Unhos e Apelação.

Esta zona tem:
- Área: 44.86 km2
- População: 149988
-- Dos quais 115936 (77%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 3343 pessoas por km2

Esta zona é maior que a anterior, e menos densa. É possível ver largas áreas no seu interior com baixa densidade populacional. É também interessante verificar que a zona mais a leste desta área, que é a UF Santa Iria de Azóia, São João da Talha e Bobadela, até está perto de uma linha ferroviária (a linha da Azambuja, operada pela CP), mas as duas estações mais próximas, Bobadela e Santa Iria, não servem adequadamente as zonas onde as pessoas vivem. Dado que a linha ferroviária já existe, e em modo *wishful thinking*, uma nova estação ou apeadeiro entre estas duas estações poderia trazer bastante gente para a ferrovia. Alternativamente, esta UF é boa candidata para um metro de superfície ou um bom serviço de autocarros que alimente as duas estações da CP já existentes.

Uma curiosidade: tecnicamente, Loures tem Metro - a fronteira entre Lisboa e Loures passa na Rua 1º de Maio, em Moscavide, e duas das entradas para a estação de Metro de Moscavide, na linha Vermelha, são no lado Norte desta rua - já no município de Loures. No entanto, este mapa mostra que há uma grande extensão de Loures, com densidade populacional razoável, sem proximidade de ferrovia.

As zonas da Portela e de Sacavém estavam também contempladas na [expansão do Metro de 2009][metro2009], neste caso com um novo ramal da linha Vermelha. Uma outra extensão, da linha Amarela para o Infantado, iria também servir o município de Loures, mas não as zonas aqui analizadas. Passaria mais a Norte, por Santo António dos Cavaleiros e pela cidade de Loures.

## Oeiras Leste
{% include map_oeste_de_monsanto.html %}

Esta zona inclui as seguintes freguesias:
- Município de Lisboa: Belém; Ajuda.
- Município de Oeiras: UF Algés, Linda-a-Velha e Cruz Quebrada-Dafundo; UF Carnaxide e Queijas.
- Município da Amadora: Alfragide.

Esta zona tem:
- Área: 31.80 km2
- População: 131819
-- Dos quais 90919 (69%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 4415 pessoas por km2


## Oeiras Oeste
{% include map_oeiras.html %}

Esta zona inclui as seguintes freguesias:
- Município de Oeiras: UF Oeiras e São Julião da Barra, Paço de Arcos e Caxias; UF Porto Salvo.
- Município de Cascais: Carcavelos e São Domingos de Rana.

Esta zona tem:
- Área: 49.34 km2
- População: 178979
-- Dos quais 92637 (52%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 3627 pessoas por km2

## Almada Oeste
{% include map_almada.html %}

Esta zona inclui as seguintes freguesias:
- Município de Almada: UF Caparica e Trafaria; UF Charneca de Caparica e Sobreda; Costa da Caparica.

Esta zona tem:
- Área: 55.96 km2
- População: 89066
-- Dos quais 73909 (83%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 1592 pessoas por km2

## Seixal
{% include map_seixal.html %}

Esta zona inclui a seguinte freguesia:
- Município do Seixal: UF Seixal, Arrentela e Aldeia de Paio Pires.

Esta zona tem:
- Área: 29.90 km2
- População: 45607
-- Dos quais 41085 (90%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 1525 pessoas por km2

## Montijo
{% include map_montijo.html %}

Esta zona inclui a seguinte freguesia:
- Município do Montijo: UF Montijo e Afonsoeiro

Esta zona tem:
- Área: 31.46 km2
- População: 41411
-- Dos quais 41411 (100%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 1316 pessoas por km2

## Quinta do Conde
{% include map_quinta_do_conde.html %}

Esta zona inclui a seguinte freguesia:
- Município de Sesimbra: Quinta do Conde.

Esta zona tem:
- Área: 14.37 km2
- População: 28092
-- Dos quais 28092 (100%) vivem a mais de 20 minutos a pé de uma estação ferroviária
- Densidade populacional: 1954 pessoas por km2

A Quinta do Conde, e a estação mais próxima (Coina), são um caso de estudo interessante. O caminho a pé entre a parte norte da Quinta do Conde e a estação de Coina *podia* ser relativamente curto se fosse mais ou menos a direito. No entanto, a existência da auto-estrada A2 impede isso, como se pode ver na imagem abaixo (captura de ecrã do Google Maps).
![Captura de ecrã]({{ site.url }}/assets/img/quinta_do_conde_coina.png)

Embora a densidade da *freguesia* seja 1954 pessoas por km2, passando o rato por cima da zona mais densa é possível ver que a densidade da zona mais urbanizada é superior a 5000 pessoas por km2 na grande maioria dos quarteirões. É portanto uma zona bastante densa, com uma estação ferroviária não tão longe assim. Pequenos investimentos em encurtar o caminho até à estação a partir da Av. 10 de Junho, uma ponte ciclopedonal sobre a A2, e criar caminhos cicláveis seguros (que ainda não existem, segundo o site [ciclovias.pt][ciclovias.pt]) para que as pessoas se desloquem até à estação de bicicleta pela Av. 10 de Junho e pela estrada N10, podem permitir servir toda esta zona e dar às dezenas de milhares de pessoas desta zona a opção de não ter carro, ou pelo menos de não o usar tantas vezes, com a poupança que daí advém.

[gsdg]: https://globaldesigningcities.org/wp-content/uploads/guides/global-street-design-guide.pdf
[metro2009]: https://pt.wikipedia.org/wiki/Metropolitano_de_Lisboa#Projetos_Anteriormente_Apresentados
[osm]: [https://www.openstreetmap.org/]
[ors]: [https://openrouteservice.org/]
[ciclovias.pt]: [https://www.ciclovias.pt/?lat=38.57706&lng=-9.04511&z=14.52900000000001&m=r&l=16]