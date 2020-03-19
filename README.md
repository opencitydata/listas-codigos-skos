En este repositorio se almacenan las listas de códigos SKOS (también denominados tesauros) usadas por el resto de vocabularios que se están desarrollando en el contexto de esta organización y que se están publicando en http://vocab.linkeddata.es/datosabiertos/.

Cada vez que se necesita crear una de estas listas, se hace referencia a ella desde el vocabulario correspondiente y se añade en este repositorio. En los casos en los que se ha utilizado alguna herramienta (por ejemplo, OpenRefine) o código software para la creación de la lista de códigos, también se incluye, para facilitar su mantenimiento.

Todas las listas de códigos son a continuación publicadas utilizando principios de _Linked Data_ para que las URIs sean derreferenciables (con el esquema de URI http://vocab.linkeddata.es/datosabiertos/kos/{sector}/{dominio}/{nombre-lista}), y también están disponibles para su consulta a través de un punto de acceso SPARQL (http://vocab.linkeddata.es/sparql).

# Listas de códigos publicadas
De momento, están publicadas las siguientes listas de códigos (organizadas de acuerdo con el sector principal de la Norma Técnica de Interoperabilidad [1] en el que son más utilizadas):

## comercio
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/cnae
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/periodo-funcionamiento
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/tipo-acceso
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/tipo-agrupacion
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/tipo-estado-tramite-licencia
* http://vocab.linkeddata.es/datosabiertos/kos/comercio/tipo-situacion

## demografia
* http://vocab.linkeddata.es/datosabiertos/kos/demografia/padron-municipal/edad
* http://vocab.linkeddata.es/datosabiertos/kos/demografia/padron-municipal/tipo-documento-identidad
* http://vocab.linkeddata.es/datosabiertos/kos/demografia/padron-municipal/tipo-local-residencia
* http://vocab.linkeddata.es/datosabiertos/kos/demografia/padron-municipal/tipo-nivel-estudio
* http://vocab.linkeddata.es/datosabiertos/kos/demografia/padron-municipal/tipo-variacion

## medio-ambiente
*	http://vocab.linkeddata.es/datosabiertos/kos/medio-ambiente/calidad-aire/tipo-estacion
*	http://vocab.linkeddata.es/datosabiertos/kos/medio-ambiente/contaminacion-acustica/emisor-acustico

## sector-publico
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/clave-nif-forma-juridica
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/estado-entidad
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/nivel-administracion
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/tipo-entidad
*	http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/servicio
*	http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/servicio/tipo-agente
*	http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/servicio/tipo-servicio
*	http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/subvencion/tipo-instrumento
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/territorio/tipo-estado
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/participacion-ciudadana/estado-propuesta
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/convenio/tipo-entidad
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/convenio/modalidad-convenio
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/convenio/variacion-convenio
* http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/convenio/tipo-convenio

## transporte
*	http://vocab.linkeddata.es/datosabiertos/kos/transporte/perfil-usuario
*	http://vocab.linkeddata.es/datosabiertos/kos/transporte/tipo-validacion
*	http://vocab.linkeddata.es/datosabiertos/kos/transporte/titulo
*	http://vocab.linkeddata.es/datosabiertos/kos/transporte/trafico/tipo-trafico
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/bicicleta-publica/tipo-estado-bicicleta
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/bicicleta-publica/tipo-estado-estacion
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/bicicleta-publica/tipo-modelo-bicicleta
* http://vocab.linkeddata.es/datosabiertos/kos/transporte/bicicleta-publica/tipo-estado-anclaje

## urbanismo-infraestructuras
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/alumbrado-publico/tipo-lampara
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/equipamiento/tipo-equipamiento
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/tipo-via
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/autobus/accesibilidad/modelo
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/autobus/accesibilidad/filas-asientos-reservados
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/autobus/tipo-equipo-asistencia
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/mobility-impairment
* http://vocab.linkeddata.es/datosabiertos/kos/urbanismo-infraestructuras/transporte/perfil-discapacidad

## general (reservado para listas que se pueden utilizar en diversos dominios)

# Uso del punto de acceso SPARQL
Como se ha apuntado anteriormente, las listas de códigos están actualmente disponibles en el punto SPARQL http://vocab.linkeddata.es/sparql, y todas ellas (así como todos los conceptos que contienen) están publicadas de acuerdo con los principios de _Linked Data_, de tal manera que sus URIs son derreferenciables.

En los próximos meses se procederá a realizar una sincronización automática de todas estas listas de códigos (hasta el momento su carga en el _triple store_ ha sido realizada de manera manual), y una unificación de todas estas listas en el mismo grafo (http://vocab.linkeddata.es/datosabiertos/kos). Por el momento, todas estas listas de códigos están distribuidas en diversos grafos.

Estas son algunas de las consultas SPARQL que se pueden realizar (se modificarán ligeramente los enlaces cuando se haya procedido a realizar el proceso de actualización automática, y se ampliarán con las peticiones que se vayan realizando):

## Obtener todas las listas de códigos publicadas, junto con el grafo donde han sido publicadas
```sparql
SELECT DISTINCT ?g ?s WHERE {
  GRAPH ?g { ?s a skos:ConceptScheme }
}
```
Enlace directo: http://vocab.linkeddata.es/sparql?default-graph-uri=&query=SELECT+DISTINCT+%3Fg+%3Fs+WHERE+%7B+GRAPH+%3Fg+%7B+%3Fs+a+skos%3AConceptScheme+%7D+%7D&format=text%2Fhtml&timeout=0&debug=on

## Obtener todos los conceptos de una lista de códigos
```sparql
SELECT DISTINCT ?s WHERE {
  ?s a skos:Concept .
  ?s skos:inScheme <http://vocab.linkeddata.es/datosabiertos/kos/sector-publico/organizacion/nivel-administracion>  
}
```
Enlace directo: http://vocab.linkeddata.es/sparql?default-graph-uri=&query=SELECT+DISTINCT+%3Fs+WHERE+%7B++%3Fs+a+skos%3AConcept+.+%3Fs+skos%3AinScheme+%3Chttp%3A%2F%2Fvocab.linkeddata.es%2Fdatosabiertos%2Fkos%2Fsector-publico%2Forganizacion%2Fnivel-administracion%3E+%7D+&format=text%2Fhtml&timeout=0&debug=on

# Referencias

[1] Guía de aplicación de la Norma Técnica de Interoperabilidad (2016) https://datos.gob.es/sites/default/files/20160726_guia_de_aplicacion_de_la_nti_reutilizacion_recursos_de_informacion_l.pdf
