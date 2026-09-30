# <h1 align="center">Linea Temporal de las funcionalidades de Liberium</h1>

Se desarrollaran todas las funciones del backend y, a aproximadamente 6 semanas del fin de desarrollo, el frontend. La 1 o 2 últimas semanas se utilizarán para debugging.

### BACKEND

1. Publicación, alquiler y venta de libros; fetch a API de libros para corroboración y autoetiquetado
2. Búsqueda de libros
3. Perfil de usuario, ajustes y personalización
4. Chats entre usuarios
5. Feed de libros
6. Favoritos
7. Foros

### FRONTEND

1. Estructura HTML y JavaScript
2. Diseño y animaciones

##
### <h1 align="center"> Notas a futuro </h1>
* Al tener un formulario, para mejorar experiencia de usuario, indicar -> "Para que tu publicación llegue a más personas, sugerimos que llenes estos breves formularios"

* Al almacenar libros, para liberar carga de la BBDD, almacenamos en 27 archivos (orden alfabético) para hacer busquedas concretas de menor carga. (si un libro empieza por "A", almacenaro en el primer archivo y ya buscar por orden alfabético en ese sub-archivo) Esto disminuirá de manera drástica los tiempos de carga de cada libro para generar publicaciones al no tener que 1. cargar miles de entradas y 2. ordenar dichas entradas cargadas.

* en BBDD, los generos se tendrán que gestionar en una relación 1 a M. Tendrémos una serie de generos ya registrados en la BBDD. En caso de que no sean suficientes, una posibilidad de contacto al equipo (nosotros) para añadir sugerencias o arreglar elementos del form.

* los chats tendran que registrarse con un identificador único para poder comprobar que los usuarios puedan correctos puedan hablar sin terceros. Esta id será generada a partir de las ID's de los dos usuarios y se "Hashea". 