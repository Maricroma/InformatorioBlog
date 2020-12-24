# InformatorioBlog
Final Project for Informatorio 2020: Spring Boot Rest API 

DESCRIPCIÓN DE LA APLICACIÓN (API)
El Informatorio planea lanzar en varias plataformas (Web, iOS y
Android) una aplicación con formato de Blogs donde varios
profesionales, profesores e inclusive alumnos podrán publicar
trabajos, noticias y mas. Para esta primera etapa se necesita del
desarrollo de una API Rest para satisfacer a todas las plataformas.
La cual deberá proveer, validar y registrar las operaciones
relacionadas a usuarios, posts (publicaciones) y comentarios.

ENTIDADES (OBJETOS DEL NEGOCIO)
De las siguientes entidades se necesita conocer y registrar
USUARIO:
● id (autogenerado)
● nombre
● apellido
● email (unico)
● password (se almacenará pero no deberá ser mostrado)
● fecha de creación (o alta)
● ciudad
● provincia
● país
De las siguientes entidades se necesita conocer y registrar
POST:
● id (autogenerado)
● título
● descripción
● contenido (cuerpo de la publicación o noticia)
● fecha de creación (o alta)
● Autor (relación con Usuario. No existen coautores)
● publicado (true o false)
De las siguientes entidades se necesita conocer y registrar
COMENTARIO:
● id (autogenerado)
● Autor (relación con Usuario)
● fecha de creación (o alta)
● comentario (no puede exceder los 200 caracteres).

OPERACIONES (SERVICIOS)
PARA USUARIO SE DEBERÁ PODER REALIZAR LAS
SIGUIENTES OPERACIÓN CON LA API
1 ALTA, BAJA Y MODIFICACIÓN
2 CONSULTA (OBTENER TODOS LOS USUARIOS) ESCONDER EL ATRIBUTO
PASSWORD DE CADA UNO
3 CONSULTA (OBTENER TODOS LOS USUARIOS DE LA CIUDAD DE
RESISTENCIA)
IDEM A #2
4 CONSULTA (OBTENER TODOS LOS USUARIOS QUE FUERON
CREADOS LUEGO DE UNA FECHA DADA)
IDEM A #2
PARA POST SE DEBERÁ PODER REALIZAR LAS SIGUIENTES
OPERACIÓN CON LA API
1 ALTA, BAJA Y MODIFICACIÓN DE POST NO SE PUEDEN AGREGAR POST
SIN AUTORES
2 CONSULTA - OBTENER TODOS LOS POST
3 CONSULTA - OBTENER TODOS LOS POST QUE CONTENGA
UNA PALABRA DADA EN EL TÍTULO
LA PALABRA PUEDE COINCIDIR EN
CUALQUIER PARTE DEL TÍTULO
4 TRAER TODOS LOS POST SIN PUBLICAR
PARA COMENTARIO SE DEBERÁ PODER REALIZAR LAS
SIGUIENTES OPERACIÓN CON LA API
1 ALTA, BAJA Y MODIFICACIÓN DE COMENTARIO NO EXISTEN COMENTARIOS
ANÓNIMOS, NI TAMPOCO
COMENTARIOS HUERFANOS (SIN
RELACIÓN A UN POST)
2 CONSULTA - OBTENER TODOS LOS COMENTARIOS DE UN
POST, CON LA OPCIÓN DE PASAR EL LIMITE DE
COMENTARIOS DESEADOS COMO MÁXIMO.
IDEM A #2. SI NO LE PASO EL LIMITE
TRAE TODOS. SI LE PASO 3, ME
TRAERÁ LOS 3 COMENTARIOS MÁS
NUEVO SOLAMENTE.
