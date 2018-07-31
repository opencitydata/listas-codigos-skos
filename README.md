En este repositorio se almacenan las listas de códigos SKOS (también denominados tesauros) usadas por el resto de vocabularios que se están desarrollando en el contexto de esta organización y que se están publicando en http://vocab.linkeddata.es/datosabiertos/. 

Cada vez que se necesita crear una de estas listas, se hace referencia a ella desde el vocabulario correspondiente y se añade en este repositorio. En los casos en los que se ha utilizado alguna herramienta (por ejemplo, OpenRefine) o código software para la creación de la lista de códigos, también se incluye, para facilitar su mantenimiento. 

Todas las listas de códigos son a continuación publicadas utilizando principios de Linked Data para que las URIs sean derreferenciables (con el esquema de URI http://vocab.linkeddata.es/datosabiertos/kos/{sector}/{dominio}/{nombre-lista}), y también están disponibles para su consulta a través de un punto de acceso SPARQL.

De momento, están publicadas las siguientes listas de códigos (organizadas de acuerdo con el sector principal de la Norma Técnica de Interoperabilidad [1] en el que son más utilizadas):

## comercio
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/cnae

## sector-publico
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/estado-entidad
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/nivel-administracion
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/tipo-entidad
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/territorio/tipo-estado

## transporte (no es un sector, y será movido a urbanismo-infraestructuras)
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/perfil-usuario
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/tipo-validacion
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/titulo

## urbanismo-infraestructuras
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/tipo-via
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/equipamiento/tipo-equipamiento
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/mobility-impairment 
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/perfil-discapacidad

## general (reservado para listas que se pueden utilizar en diversos dominios)



# Referencias

[1] Guía de aplicación de la Norma Técnica de Interoperabilidad (2016) https://datos.gob.es/sites/default/files/20160726_guia_de_aplicacion_de_la_nti_reutilizacion_recursos_de_informacion_l.pdf
