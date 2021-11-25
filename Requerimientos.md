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
