## ARQUITECTURA Y JUSTIFICACIÓN

|      | Microservicios|Por eventos  |
| ----------- | ----------- |-----------|
| Agilidad      | 👍       |👍|
| Despliegue   | 👍        |👍|
| Pruebas   | 👎        |👎|
| Desempeño   | 👎       |👎|
| Escalabilidad  |👍       |👎|
| Facil de desarrollar |👍|👎|


# Consideraciones:
- Personas externas al ITAM pueden entrar a proponer proyectos
- Se espera que la mayoría de lxs alumnxs voten por proyectos >5000 usuarios: Despliegue y desempeño
- Se busca tener un seguimiento continuo del proyecto: Desempeño
- Hay un número tope de proyectos por semestre (no pueden haber más de 20 proyectos en curso) : No escalabilidad
- Los lineamientos pueden cambiar: Agilidad

Dado que la aplicación no necesariamente tendrá cambios drásticos seguidos porque en las primeras semanas del semestre se pondrán a votación los proyectos para ese año, y al cerrarse la votación solo se podrá ver el desarrollo y los proyectos pensados para el próximo año (que tendrán que irse actualizando cada dos meses), se pensó que no es tan necesaria una escalabilidad de la página en general, pero por proyecto se le podrían agregar muchas cosas a lo largo que escala el proyecto. Sin embargo, eso sería independiente de la aplicación como tal. También lxs alumnxs no van a estar en la app 24/7, de hecho se espera que las veces que se visite, sea cuando sean las elecciones y de vez en cuando que quieran ver el desarrollo de proyectos, pero no es una app que sea de prioridad alta para lxs alumnxs durante el semestre, por lo que se utilizaría cuando la necesiten.

Mezcla de Microservicios y por Eventos:
- Microservicios:
Se escalarían cosas depende del proyecto 
El despliegue es bueno y al no ser algo tan prioritario para lxs alumnxs, puede que si no se despliega rápido, se pierda interés.
Al tener diferentes microservicios podemos dividir el desarrollo de varios de ellos y así es más fácil para desarrollar.
- Por eventos
Complementa muy

