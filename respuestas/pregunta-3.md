MATCH (p1:Persona)-[:TRABAJA_EN]->(e:Empresa)<-[:TRABAJA_EN]-(p2:Persona)
WHERE p1 <> p2
RETURN p1.nombre, p2.nombre, e.nombre