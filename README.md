# contenedorDNS
Repositorio con el contenedor DNS Bind9
version: versión de docker-compose 
services: define los servicios que ofrece el contenedor
 asir_bind9: comienzo del contenido del contenedor "asir_bind9"
   container_name: nombre del contenedor
   image: ruta de la imagen
   ports: en esta sección se indican los puertos del contenedor
     - 5300:53/udp  (puerto udp)
     - 5300:53/tcp  (puerto tcp)
   volumes: en esta sección se indica la ruta del .conf y del .yml
     - /home/asir2a/Escritorio/SRI/tuto/bind9/conf:/etc/bind
     - /home/asir2a/Escritorio/SRI/tuto/bind9/zonas:/var/lib/bind
