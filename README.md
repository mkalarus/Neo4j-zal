Neo4j-zal
=========

zadanie z Neo4j
Poniżej moja baza w której wykorzystałem część danych na których pracuję

![graf bazy](baza1.png)

Poniżej przykładowe polecenia tworzące elementy bazy

CREATE (M2_06:Proba {stacja:'M2', zebrane:'04.07.2006', warstwa:'10-0m'})
CREATE (Pn:takson {name:'Pseudocalanus', stadium:'N'})

Oraz relacje

CREATE (Ac1)-[:WYSTEPOWAL {licz:[607]}]->(M2_06)

Przykładowe łączenie

MATCH (aca_c: takson {name:'Acartia', stadium:'C1'})-[:WYSTEPOWAL]->(aca_c_wyst) RETURN aca_c, aca_c_wyst

