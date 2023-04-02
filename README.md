# Análisis de fuga de empleados con Machine Learning

A raíz de los datos de abandono de empleados en la empresa, vamos a realizar una serie de análisis para identificar mejor el problema y hallar posibles soluciones.

### Primera parte: identificación del problema

Comenzamos haciendo una limpieza y primera exploración de los datos. Los datos incluyen características del empleado, si este abandonó o no la empresa y otros datos de satisfacción. 

Analizando al grupo de trabajadores que dejaron la empresa, hemos construido un perfil medio. 
* Bajo nivel educativo
* Soltero
* Trabaja en ventas
* Bajo salario
* Alta carga de horas extras

Así pues, los actuales empleados que más se acerquen a este perfil son los que estarán en un mayor riesgo de abandono.

### Segunda parte: impacto económico

Con el fin de cuantificar el problema, y valorar mejor sobre qué grupo de empleados merece la pena priorizar, vamos a estimar las pérdidas que se estiman por cada empleado.
Siguiendo unas estimaciones de un estudio del Center for American Progress, la estimación nos dice que:
* en el último año las pérdidas por aband ono se estiman 2 719 005.91€
* las pérdidas de empleados que no estaban motivados fueron 368 672.69€

Podemos estimar el ahorro que supondría retener a un porcentaje de estos empleados:
* 30% - 815 701€
* 20% - 543 801€
* 10% - 271 900€

Hemos visto también que, sobre el grupo de mayor riesgo (representantes de ventas), retener un 30% (5 empleados) supondría un ahorro de 37 447.22€

De este modo, podemos estimar un presupuesto para acciones de retención por cada departamento o perfil. 


### Tercera parte: modelo de machine learning





