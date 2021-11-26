
# TEST PLAN
## 1 TEST PLAN IDENTIFIER 

El test plan identifier de este documento es plan_de_calidad_PROYECTA_ITAM_v1

Fecha: 25/11/21 

Autorxs:
Equipo Chaviza

Santiago Delgado

Ana Cristina Sánchez

Lucia Lizardi

Juan I. Hernández

## 2 REFERENCIAS

* [Requerimientos](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Requerimientos.md)
* [Arquitectura y justificacion](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Arquitectura%20y%20Justificaci%C3%B3n.md)
* [Metodología y justificación](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Metodolog%C3%ADaYJustificacion.md)
* [Propuesta económica](https://app.moqups.com/MGHKpHQoFzL0tnLWQSHoPrmzQogyRgHn/view/page/a8310d123)
* [Código](https://docs.google.com/spreadsheets/d/1ln8IqfAp9rtSpbkd0Omaz1Uzz7hbInp1jhrrJ3ZuMsk/edit?usp=sharing)

## 3 INTRODUCCIÓN

Este plan tiene el propósito de trazar las directrices para el desarrollo y primera implementación de Proyecta ITAM. El enfoque específico es mostrar las metodologías, vistas, funcionalidades y requerimientos, costos y riesgos, necesario para realizar la aplicación

## 4 TEST ITEMS (FUNCIONALIDADES) 

Las funcionaliades que se probarán serán:
* Ingresar a la página
* Registrarse 
* Escribir un cometario en un proyecto en específico
* Publicar un comentario en un proyecto en específico
* Votar por un proyecto en específico
* Navegar por los comentarios existentes.

## 5 RIESGOS PARA EL SOFTWARE 

Los riesgos relacionados al software que pudimos detectar como posibles son:

Errores en los servidores donde este desplegado el servicio

Errores en servicios y bibliotecas auxiliares

Errores y vunerabilidades no detectadas, o posteriores a haber terminado el proyecto

Errores humanos al momento de dar mantenimiento

Errores relacionados con las bases de datos que se utilicen o una creación inicial errónea


## 6 FEATURES POR PROBAR
Las funcionalidades que se probarán desde el punto de vista del usuario son las siguientes:
* Página de inicio
    *   Ingreso de usuario
    *   Ingreso de contraseña
    *   (Acceso a la base de datos)
* Registro
    *   Ingreso de usuario
    *   Ingreso de correo electrónico 
    *   Ingreso de contraseña
    *   Ingreso de confirmación de contraseña
    *   (Actualización de la base de datos) 
* Votar
    * (Actualización de la base de datos) 

Es importante probarlas desde este ángulo porque el usuario es el que se encargará de manejarlas, por lo que es importante que se hagan lo más sencillas e intuitivas posibles.
La votación es el objetivo principal de la página, por lo que no puede haber errores a la hora de que algún usuario vote por un proyecto.
De igual manera, el ingresar a la aplicación es importante para que todo el quien lo desee pueda votar. 

## 7 FEATURES NOT TO BE TESTED 
Las funcionalidades que no se probarán desde el punto de vista del usuario son las siguientes:
* Visualización de comentarios
    *   (Acceso a la base de datos)
* Comentar
    *   Ingreso de comentario
    *   (Actualización de la base de datos) 


Estas funcionalidades no se probaran desde éste ángulo debido a que son secundarias. Si es importante que los usuarios puedan votar, pero tiene más prioridad que puedan votar. Es por esto que los recursos se enfocarán en la prueba de voto antes que en comentar y visualizar comentarios.   

## 8 ESTRATEGIA 

Antes de comenzar el proyecto verificaremos que cada miembro del equipo conoce su rol durante el proyecto, y que está capacitado para él. Se realizara un análisis detallado de que tecnologías usar y solo se tomaran las que el equipo esta seguro que puede implementar (que conoce). Será necesario que cada programador cuente con la disponibiblidad y una computadora con acceso a internet donde pueda escribir código. Una vez que se cuenten con estos requerimientos iniciales se realizará una evaluación exhaustiva con el ITAM para definir los objetivos del proyecto. Finalizado esto se comenzará con las metodologías ágiles a trabajar y se espera que al final de cada sprint se muestren avances significativos y testeados para la consecución del proyecto.

## 9 ITEM PASS/FAIL CRITERIA (PASA/NO PASA LA PRUEBA)

Como consideramos que la aplicación no es muy compleja en requerimientos técnicos, no aceptaremos código con errores por pequeños que sean en la versión final. Buscaremos detectar cada bug o problema en el testeo previo a subir cada funcionalidad.

## 10 SUSPENSION CRITERIA AND RESUMPTION REQUIREMENTS (CRITERIA DE SUSPENSIÓN)

Si detectamos un problema que no podemos resolver, que pueda ocasionar problemas a futuro, que entre en conflicto con nuestras tecnologías principales o que vulnere sin solución la seguridad del proyecto lo eliminaremos.

Así como alguna situación en la que se vean comprometida la seguridad de nuestrxs usuarixs. Hasta no solucionarse no retomaríamos.

## 11 TEST DELIVERABLES (ENTREGABLES)

Se entregará un plan de testeo, casos de testeo, especificaciones funcionales, especificaciones de diseño, reportes, prototipos, y observaciones importantes.

## 12 REMAINING TEST TASKS (TAREAS DE PRUEBAS)

Las que sean detectadas en cada iteración ágil del proyecto con los prototipos que se vayan creando.

## 13 ENVIRONMENTAL NEEDS  (REQUERIMIENTOS DE AMBIENTE)

Como tal no detectamos requerimientos ambientales que no sean normales en el desarrollo de una aplicación sencilla de software. Es decir, no necesitamos software o hardware especial. No detectamos requerimientos de energía inusuales ni software de soporte antiguo. Lo único que necesitamos son servidores para el despliegue y donde alojemos el proyecto y computadoras normales para trabajo que usarán los programadores.

## 14 STAFFING AND TRAINING NEEDS (ENTRENAMIENTO PARA EL STAFF) 

Se necesitará que todos los miembros tengan un conocimiento suficiente de programación de aplicaciones web. Se necesitará un especialista entrenado en pruebas para la aplicación, las pruebas como tal, se definiran antes de iniciar el proyecto entre todo el equipo y con conocimiento profundo y previo de los requerimientos del empleador. Es importante que exista un especialista en diseño de aplicaciones y otro en experiencia de usuario, pueden ser la misma persona. Debe existir un lead developer experimentado que guié el proyecto.

## 15 RESPONSIBILITIES (RESPONSABILIDADES)

El encargado del proyecto es el Project Manager, luego el tendrá que asignarle las responsabilidades correspondientes a cada miembro del proyecto y verificar que sean cumplidas.


## 16 SCHEDULE (AGENDA)

La agenda se decidirá conforme se den las iteraciones correspondientes y de acuerdo a las restricciones que ponga el empleador (ITAM).

## 17 PLANNING RISKS AND CONTINGENCIES 

Hemos detectado riesgos en cuanto a la planeación en caso de que algún miembro tenga problemas con su equipo de trabajo y no se pueda dar un reemplazo rápido.
También existen riesgos debido a la salud de los integrantes, en especial, por la pandemia actual.
Existen riesgos por problemas que no se hayan detectado o aparezcan debido a errores humanos más adelante en el proyecto y condicionen su consecución.

## 18 APPROVALS 

Solo los integrantes originales del equipo tienen autorización para modificar el proyecto, si en un momento posterior existen más integrantes tendrán que consultarlo con los integrantes originales. Estos integrantes son:

Santiago Delgado

Ana Cristina Sánchez

Lucia Lizardi

Juan I. Hernández
