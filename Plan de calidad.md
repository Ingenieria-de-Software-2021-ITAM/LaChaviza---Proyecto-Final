
# TEST PLAN
## 1 TEST PLAN IDENTIFIER 
Some type of unique company generated number to identify this test plan, its level and the level of software that it is related to.  Preferably the test plan level will be the same as the related software level.  The number may also identify whether the test plan is a Master plan, a Level plan, an integration plan or whichever plan level it represents. This is to assist in coordinating software and testware versions within configuration management. Keep in mind that test plans are like other software documentation, they are dynamic in nature and must be kept up to date.  Therefore, they will have revision numbers. You may want to include author and contact information including the revision history information as part of either the identifier section of as part of the introduction. 

## 2 REFERENCES

* [Requerimientos](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Requerimientos.md)
* [Arquitectura y justificacion](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Arquitectura%20y%20Justificaci%C3%B3n.md)
* [Metodología y justificación](https://github.com/Ingenieria-de-Software-2021-ITAM/LaChaviza-ProyectoFinal/blob/main/Metodolog%C3%ADaYJustificacion.md)
* [Propuesta económica](https://app.moqups.com/MGHKpHQoFzL0tnLWQSHoPrmzQogyRgHn/view/page/a8310d123)
* [Código](https://docs.google.com/spreadsheets/d/1ln8IqfAp9rtSpbkd0Omaz1Uzz7hbInp1jhrrJ3ZuMsk/edit?usp=sharing)

## 3 INTRODUCTION

Este plan tiene el propósito de trazar las directrices para el desarrollo y primera implementación de Proyecta ITAM. El enfoque específico es mostrar las metodologías, vistas, funcionalidades y requerimientos, costos y riesgos, necesario para realizar la aplicación

## 4 TEST ITEMS (FUNCTIONS) 

Las funcionaliades que se probarán serán:
* Ingresar a la página
* Registrarse 
* Escribir un cometario en un proyecto en específico
* Publicar un comentario en un proyecto en específico
* Votar por un proyecto en específico
* Navegar por los comentarios existentes.

## 5 SOFTWARE RISK ISSUES 
Identify what software is to be tested and what the critical areas are, such as: A. Delivery of a third party product. B. New version of interfacing software C. Ability to use and understand a new package/tool, etc. D. Extremely complex functions  E. Modifications to components with a past history of failure F. Poorly documented modules or change requests There are some inherent software risks such as complexity; these need to be identified.   A. Safety B. Multiple interfaces C. Impacts on Client D. Government regulations and rules Another key area of risk is a misunderstanding of the original requirements. This can occur at the management, user and developer levels. Be aware of vague or unclear requirements and requirements that cannot be tested. The past history of defects (bugs) discovered during Unit testing will help identify potential areas within the software that are risky.  If the unit testing discovered a large number of defects or a tendency towards defects in a particular area of the software, this is an indication of potential future problems.  It is the nature of defects to cluster and clump together.  If it was defect ridden earlier, it will most likely continue to be defect prone. One good approach to define where the risks are is to have several brainstorming sessions. § Start with ideas, such as, what worries me about this project/application.

## 6 FEATURES TO BE TESTED 
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

## 8 APPROACH (STRATEGY)

Antes de comenzar el proyecto verificaremos que cada miembro del equipo conoce su rol durante el proyecto, y que está capacitado para él. Se realizara un análisis detallado de que tecnologías usar y solo se tomaran las que el equipo esta seguro que puede implementar (que conoce). Será necesario que cada programador cuente con la disponibiblidad y una computadora con acceso a internet donde pueda escribir código. Una vez que se cuenten con estos requerimientos iniciales se realizará una evaluación exhaustiva con el ITAM para definir los objetivos del proyecto. Finalizado esto se comenzará con las metodologías ágiles a trabajar y se espera que al final de cada sprint se muestren avances significativos y testeados para la consecución del proyecto.

## 9 ITEM PASS/FAIL CRITERIA
What are the Completion criteria for this plan?  This is a critical aspect of any test plan and should be appropriate to the level of the plan. § At the Unit test level this could be items such as: § All test cases completed. § A specified percentage of cases completed with a percentage containing some number of minor defects. § Code coverage tool indicates all code covered. § At the Master test plan level this could be items such as: § All lower level plans completed. § A specified number of plans completed without errors and a percentage with minor defects. This could be an individual test case level criterion or a unit level plan or it can be general functional requirements for higher level plans. What is the number and severity of defects located? § Is it possible to compare this to the total number of defects?  This may be impossible, as some defects are never detected. § A defect is something that may cause a failure, and may be acceptable to leave in the application. § A failure is the result of a defect as seen by the User, the system crashes, etc.

## 10 SUSPENSION CRITERIA AND RESUMPTION REQUIREMENTS
Know when to pause in a series of tests. § If the number or type of defects reaches a point where the follow on testing has no value, it makes no sense to continue the test; you are just wasting resources. Specify what constitutes stoppage for a test or series of tests and what is the acceptable level of defects that will allow the testing to proceed past the defects. Testing after a truly fatal error will generate conditions that may be identified as defects but are in fact ghost errors caused by the earlier defects that were ignored. 

## 11 TEST DELIVERABLES 
What is to be delivered as part of this plan? § Test plan document. § Test cases. § Test design specifications. § Tools and their outputs. § Simulators. § Static and dynamic generators. § Error logs and execution logs. § Problem reports and corrective actions. One thing that is not a test deliverable is the software itself that is listed under test items and is delivered by developmen

## 12 REMAINING TEST TASKS
If this is a multi-phase process or if the application is to be released in increments there may be parts of the application that this plan does not address.  These areas need to be identified to avoid any confusion should defects be reported back on those future functions.  This will also allow the users and testers to avoid incomplete functions and prevent waste of resources chasing non-defects. If the project is being developed as a multi-party process, this plan may only cover a portion of the total functions/features. This status needs to be identified so that those other areas have plans developed for them and to avoid wasting resources tracking defects that do not relate to this plan. When a third party is developing the software, this section may contain descriptions of those test tasks belonging to both the internal groups and the external groups. 

## 13 ENVIRONMENTAL NEEDS  

Como tal no detectamos requerimientos ambientales que no sean normales en el desarrollo de una aplicación sencilla de software. Es decir, no necesitamos software o hardware especial. No detectamos requerimientos de energía inusuales ni software de soporte antiguo. Lo único que necesitamos son servidores para el despliegue y donde alojemos el proyecto y computadoras normales para trabajo que usarán los programadores.

## 14 STAFFING AND TRAINING NEEDS 

Se necesitará que todos los miembros tengan un conocimiento suficiente de programación de aplicaciones web. Se necesitará un especialista entrenado en pruebas para la aplicación, las pruebas como tal, se definiran antes de iniciar el proyecto entre todo el equipo y con conocimiento profundo y previo de los requerimientos del empleador. Es importante que exista un especialista en diseño de aplicaciones y otro en experiencia de usuario, pueden ser la misma persona. Debe existir un lead developer experimentado que guié el proyecto.

## 15 RESPONSIBILITIES 

El encargado del proyecto es el Project Manager, luego el tendrá que asignarle las responsabilidades correspondientes a cada miembro del proyecto y verificar que sean cumplidas.

## 16 SCHEDULE
Should be based on realistic and validated estimates.  If the estimates for the development of the application are inaccurate, the entire project plan will slip and the testing is part of the overall project plan. § As we all know, the first area of a project plan to get cut when it comes to crunch time at the end of a project is the testing.  It usually comes down to the decision, ‘Let’s put something out even if it does not really work all that well’. And, as we all know, this is usually the worst possible decision. How slippage in the schedule will to be handled should also be addressed here. § If the users know in advance that a slippage in the development will cause a slippage in the test and the overall delivery of the system, they just may be a little more tolerant, if they know it’s in their interest to get a better tested application. § By spelling out the effects here you have a chance to discuss them in advance of their actual occurrence. You may even get the users to agree to a few defects in advance, if the schedule slips. At this point, all relevant milestones should be identified with their relationship to the development process identified.  This will also help in identifying and tracking potential slippage in the schedule caused by the test process. It is always best to tie all test dates directly to their related development activity dates.  This prevents the test team from being perceived as the cause of a delay.  For example, if system testing is to begin after delivery of the final build, then system testing begins the day after delivery.  If the delivery is late, system testing starts from the day of delivery, not on a specific date.  This is called dependent or relative dating. 

## 17 PLANNING RISKS AND CONTINGENCIES
What are the overall risks to the project with an emphasis on the testing process? § Lack of personnel resources when testing is to begin. § Lack of availability of required hardware, software, data or tools. § Late delivery of the software, hardware or tools. § Delays in training on the application and/or tools. § Changes to the original requirements or designs. Specify what will be done for various events, for example: § Requirements definition will be complete by January 1, 19XX, and, if the requirements change after that date, the following actions will be taken. § The test schedule and development schedule will move out an appropriate number of days.  This rarely occurs, as most projects tend to have fixed delivery dates. § The number of test performed will be reduced. § The number of acceptable defects will be increased. § These two items could lower the overall quality of the delivered product. § Resources will be added to the test team. § The test team will work overtime. § This could affect team morale. § The scope of the plan may be changed. § There may be some optimization of resources.  This should be avoided, if possible, for obvious reasons. 
IEEE Test Plan Outline Foundation Course in Software Testing Prepared by Systeme Evolutif Limited Page 8 § You could just QUIT.  A rather extreme option to say the least. Management is usually reluctant to accept scenarios such as the one above even though they have seen it happen in the past. The important thing to remember is that, if you do nothing at all, the usual result is that testing is cut back or omitted completely, neither of which should be an acceptable option.

## 18 APPROVALS

Solo los integrantes originales del equipo tienen autorización para modificar el proyecto, si en un momento posterior existen más integrantes tendrán que consultarlo con los integrantes originales. Estos integrantes son:
Santiago Delgado
Ana Cristina Sánchez
Lucia Lizardi
Juan I. Hernández
