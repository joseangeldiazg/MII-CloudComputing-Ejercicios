#Ejercicios del tema 1 de Cloud Computing

##Ejercicio 1: Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?

El proyecto fue presentado como proyecto final para la asignatura de Programación Web del grado en Ingeniería Informática y consistía en un sistema de gestión de cursos online donde había varios roles de usuarios, entre admin, profesores y alumnos con ciertos servicios y funcionalidades cada uno. El patrón que usaba era el modelo cliente-servidor. Para evolucionar a un patrón de tipo micreoservicios, deberíamos abstraer cada uno de los servicios que la aplicación ofrece y desplegarlos en la nube, por ejemplo, podríamos obtener el servicio de base de datos y desplegarlo independientemente de todos los demás, idem con todos los demás servicios como subida de documentos, alta de tareas, creación de usuarios. Todos estos servicios deberíamos comunicarlos entre si por algún API-REST y tendríamos lista nuestra app según la arquitectura microservicios.  

##Ejercicio 2: En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?

Si que se podrían usar diferentes lenguajes. Al haberla definido posteriormente como una arquitectura microservicios podríamos implemnetar cada uno de estos servicios acorde al lenguaje más adecuado, pero teniendo en cuenta la supuesta adaptación de una web que estaba en su mayoría escrita en php y javascript quizá debiéramos centrarnos en estos y algún framework sobre ellos.

Respecto a los almacenes de datos, en el inicio se uso mySQL, por lo que quizá pudiera también adaptarse a la nube algún almacén de datos basado en SQL y no tener que re adaptar todo a almacenes noSQL, ya que los datos que manejaría la aplicación estaban a priori correctamente fijados y toda la base de datos se diseñó en base a ellos. 
