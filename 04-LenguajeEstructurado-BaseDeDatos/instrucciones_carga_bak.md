# 1. Crear la carpeta dentro del contenedor
docker exec -it -u root <nombre_o_id_del_contenedor> mkdir -p /var/opt/mssql/back

# 3. Copiar tu archivo .bak
docker cp /ruta/en/tu/pc/respaldo.bak <nombre_o_id_del_contenedor>:/var/opt/mssql/backup/

# Ignora todo lo que esté dentro de la carpeta data
data/