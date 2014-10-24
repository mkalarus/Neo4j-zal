MATCH (aca_c: takson {name:'Acartia', stadium:'C1'})-[:WYSTEPOWAL]->(aca_c_wyst) RETURN aca_c, aca_c_wyst

#usuwanie wszystkiego

MATCH (n)
OPTIONAL MATCH (n)-[r]-()
DELETE n,r
