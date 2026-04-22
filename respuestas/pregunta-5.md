MATCH (p:Persona)-[r:AMIGO_DE]-()
RETURN p.nombre, count(r) AS apariciones
ORDER BY apariciones DESC
LIMIT 1