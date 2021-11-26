## 1. Introducción

### 1.1 Propósito

El proyecto consiste de un sistema de consulta de proyectos para la universidad ITAM. El objetivo es crear una plataforma que se ajuste a las necesidades de lxs alumnxs que buscan informarse acerca de los proyectos que desarrollan sus compañerxs. La propuesta se concentra en eliminar dificultades para el alumnado cuando estén buscando los proyectos. El software se usara como herramienta para buscar información a través de consultar proyectos. Nuestro software busca quitar complicaciones y crear una experiencia amigable para lxs alumnxs para que puedan desarrollar su conocimiento.

### 1.2 Convenciones del Documento

Este documento utiliza las convenciones generales de ReadMe de github utilizando el formato markdown.

### 1.3 Audiencia y Sugerencias de Lectura

Este documento está diseñado principalmente para las personas con acceso a modificación de código. Esto para que dichas personas comprendan el funcionamiento del sistema y las posibles consecuencias de modificar el código. Lxs alumnxs y maestrxs no cuentan con dicho tipo de permiso, ya que su acceso no modifica la parte nuclear del sistema. La sugerencia de lectura para este documento es lineal. El documento se divide en secciones que va de lo general a lo particular.

### 1.4 Definición del Producto

El sistema se basa principalmente en dejar a lxs alumnxs buscar proyectos de su interés, o que tengan que ver con las materias que llevan o van a llevar. Al acercar el conocimiento del alumnado al resto de lxs alumnxs se abre un nuevo canal de comunicación que se basa en información relevante.

### 1.5 Referencias

[Documento IEEE](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Plan%20de%20calidad.md)

## 2. Descripción general

### 2.1 Perspectiva del producto

### 2.2 Funcionalidad del producto
La principal funcionalidad del proyecto es ser una plataforma para la Comunidad ITAM en la cual lxs alumnxs puedan proponer y votar por proyectos para que se lleven a cabo en el ITAM. Así como darle seguimiento a los que ya habían sido seleccionados anteriormente.

Será una aplicación web que contará con un login, un catálogo de proyectos por 

### 2.3 Clases de Usuario y características
Se tomaron en cuenta las siguientes clases:
- Alumnx: Clase General de alumnxs en la cual se encuentran los datos básicos del alumnx del ITAM como nombre, CU, carrera, mail.
- Alumnx votante: Alumnx unicamente votante. Hereda la clase Alumnx y cuenta con un atributo de que le permite votar por cualquier proyecto.
- Alumnx Owner: Alumnx proponiendo proyecto. Hereda la clase Alumnx pero no puede votar por su proyecto. Así mismo, este alumnxs cuenta con un atributo que le muestra cuántos proyectos activos tiene. 
- Proyecto: Clase del proyecto con atributos: Nombre de proyecto, Tipo de proyecto, Votos, Esta Activo, Fecha De Propuesta, Fecha De Implementación, Aprobación, Descripción y Owners (lxs dueños del proyecto).
- Owner Externo: Solo es posible si la persona externa pertenece a un equipo de Ownners itamitas. Atributos: Nombre, email, teléfono, proyecto.


### 2.4 Ambiente de operaciones
Al ser una aplicación web, esta correrá en todos los buscadores de internet. 

### 2.5 Limitaciones de diseño e implementación
Por 

### 2.6 Documentación para usuarix
- [READ ME](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/README.md)
- [MANUAL DE USUARIO CON CÓDIGO](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/C%C3%B3digo.md)
### 2.7 Supuestos 

- Lxs alumnxs pueden votar.
- Tanto personas externas como alumnxs pueden proponer proyectos.
- Se esperará un máximo de 8000 votos de alumnxs, si se cuenta a toda la población estudiantil.
- La plataforma necesitará hacer cambios en un tiempo definido. Cada año obligatoriamente para que se propongan más proyectos y se irá actualizando cada 3 meses para ver el desarrollo de los proyectos activos.
- Todxs lxs usuarixs cuentan con conexión a internet y una computadora para poder acceder a la plataforma.

## 3. Requerimientos de Interfaz Externos

### 3.1 Interfaces de Usuarix

Este proyecto cuenta con una interfaz de usuarix solamente en el inicio del software y al realizar tu voto y/o comentario. El proyecto no cuenta con un diseño ni funcionamiento perzonalizado. Con esto nos referimos a que no cuenta con una interfaz de perfil.

### 3.2 Interfaces de Hardware

Este proyecto, por el momento, va a poder ser accedido en cualquier dispositivo que tenga conexión al internet. El diseño de la página esta creado para un monitor tipo computadora por lo cual en dispositivos más pequeños el diseño no será tan comodo como sucede con muchas otras páginas. Lo esencial de la herramienta puede ser realizado pero los botones pueden resultar más pequeños. 

### 3.3 Interfaces de Software

Este proyecta cuenta con cinco interfaces que cumplen con ciertas funcionalidades que componen el objetivo de la herramienta. La primera interfaz consiste en el ingreso de las credenciales del estudiante para hacer log-in, estos ya previamente dados de alta en el sistema. La interfaz principal es la segunda. Es una ventana que muestra en forma de matriz los proyectos que estan disponibles. Al ingresar a un proyecto se presenta la tercera interfaz que expone la información acerca del proyecto. Esta interfaz tiene la conexión a las dos últimas que se encargan de manejar los procesos de las votaciones así como de la publicación de comentarios.

### 3.4 Interfaces de Comunicación

La interfaz de comunicación para nuestro proyecto será unicamente la ventana para publicar comentarios. Debido a que el objetivo principal es la de informar el rasgo social de la aplicación se limita a esta funcionalidad. Lxs alumnxs pueden expresarse pero el mensaje es para todxs.

## 4. Funcionalidades

### 4.1 Consulta de las Proyectos

#### 4.1.1 Descripción y Prioridad

Esta funcionalidad consiste en permitir a lxs alumnxs consultar los proyectos que sean de su interés. Lxs alumnxs pueden aprovechar esta funcionalidad para acceder a información proporcionada por otrxs alumnxs. Esta funcionalidad es de prioridad alta ya que sin ella el alumnado no puede acceder a los proyectos y aprovechar la herramienta.

#### 4.1.2 Secuencia de Respuestas

    1. Estudiante ingresa a la página de inicio del sistema
    2. Estudiante navega por la matriz de diferentes proyectos a los que quiera acceder.

#### 4.1.3 Requerimientos Funcionales

    - REQ-1: La sección para consultar proyectos tiene que ser la 
             primera pantalla en aparecer al iniciar sesión.
    - REQ-2: La consulta de los proyectos tiene que ser intuitiva para el usuarix 
             teniendo en cuenta los diferentes temas que abarcan los proyectos.
    - REQ-3: Regresar al menú principal tiene que ser un proceso sencillo de realizar.
    - REQ-4: Se tiene que poder agregar marcadores a los proyectos que el alumnx desee.

### 4.2 Votación por Proyectos

#### 4.2.1 Descripción y Prioridad

Esta funcionalidad tiene como objetivo permitir a lxs alumnxs votar por los proyectos que consideren interesantes y bien hechos. Esta herramienta permite que los proyectos que destacan entre lxs alumnxs puedan ser reconocidos por su esfuerzo. Los resultados de la votación pueden ser vistos por el usuarix. Esta funcionalidad es de prioridad media ya que es importante pero no esencial para la consulta de los proyectos.

#### 4.2.2 Secuencia de Respuestas

    1. Estudiante ingresa desde la página de inicio del sistema.
    2. Estudiante se dirige a un proyecto de su interés y lo abre para investigar.
    3. Estudiante selecciona el botón de votar situado abajo de el abstracto del proyecto.
        3.1. Estudiante selecciona el botón de votaciones en la parte superior de la ventana.
        3.2  Estudiante regresa al abstracto del proyecto.
    4. Estudiante cierra ventana confirmando el registro de su voto.

#### 4.2.3 Requerimientos Funcionales

    - REQ-1: El botón para poder votar tiene que ser fácil de encontrar y 
             cerca del final del texto descriptivo del proyecto.
    - REQ-2: Al votar debe invocarse una ventana que confirme que la votación fue exitosa.
    - REQ-3: Se puede votar por todos los proyectos.
    - REQ-4: El botón para regresar a la ventana del proyecto.
### 4.3 Escribir Comentarios sobre el Proyecto

#### 4.3.1 Descripción y Prioridad

Esta funcionalidad se basa en permitir a lxs alumnxs escribir comentarios acerca del proyecto que decidieron investigar. La implementación de esta funcionalidad crea un ambiente de discusión en el que se pueden expresar distintas opiniones sobre el tema que toca el proyecto en cuestión. Esta funcionalidad tiene prioridad baja ya que no es esencial para el uso de la herramienta. De igual manera, no es una funcionalidad importante para el planteamiento del proyecto pero la integración de esta funcionalidad es una gran adición a la herramienta.

#### 4.3.2 Secuencia de Respuestas

    1. Estudiante ingresa desde la página de inicio del sistema.
    2. Estudiante se dirige a un proyecto de su interés y lo abre para investigar.
    3. Estudiante selecciona el botón llamado comentarios.
    4. Estudiante escribe el comentario que tiene acerca del proyecto para compartir con la comunidad.

#### 4.3.2 Requerimientos Funcionales

    - REQ-1: El botón para acceder a la sección de comentarios del software debe ser claro e intuitivo de encontrar.
    - REQ-2: Un espacio de texto para que el alumnx ponga su comentario.
    - REQ-3: Se tiene que mostrar los comentarios de otrxs alumnxs.
    - REQ-4: El botón que permita regresar a la ventana del proyecto.
    
## 5. Requerimientos No Funcionales 

### 5.1 Requerimientos de Rendimiento

El sistema debe ser capaz de aguantar a 5,000 usuarios al mismo tiempo. Esto será puesto a prueba por nuestro equipo de DevOps. Con una herramienta adicional podrán realizar las implementaciones necesarias para que varixs estudiantes puedan estar realizando su votación o publicando comentarios.

Toda funcionalidad dentro del sistema debe contestar al usuarix en menos de tres segundos. El software también tiene que actualizar la base de datos de las votaciones y comentarios en menos de tres segundos.

### 5.2 Requerimientos de Buen Uso 

- El tiempo de aprendizaje del sistema por parte de cada usuarix debe ser de una hora.
- La tasa de errores cometidos por el usuarix debe ser del 1% en todas las transacciones ejecutadas dentro del sistema.
- El sistema debe poseer interfaces gráficas bien formadas e intuitivas.

### 5.3 Requerimientos de Seguridad

- Los permisos de acceso al sistema podrán ser cambiados solamente por el administrador de acceso a datos.
- Todas las comunicaciones externas entre servidores de datos, aplicación y cliente del sistema deben estar encriptadas utilizando el algoritmo RSA.
- Si se identifican ataques de seguridad o brecha del sistema, el mismo no continuará operando hasta ser desbloqueado por un administrador de seguridad.
- Se llevará registros de lxs usuarixs. Dichos registros solamente podrán ser accedidos en caso de alguna anomalía en la plataforma.

### 5.4 Atributos de Calidad de Software

- El sistema debe tener una disponibilidad del 99,99% de las veces en que un usuario intente accederlo.
- El promedio de duración de fallas no podrá ser mayor a 15 minutos.
- La probabilidad de falla del Sistema no podrá ser mayor a 0,05.
