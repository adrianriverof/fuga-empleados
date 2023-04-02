# Análisis de fuga de empleados con Machine Learning

A raíz de los datos de abandono de empleados en la empresa, vamos a realizar una serie de análisis para identificar mejor el problema y hallar posibles soluciones.

### Primera parte: identificación del problema ([Notebook](https://github.com/adrianriverof/fuga-empleados/blob/main/1_identificacion_problema.ipynb))

Comenzamos haciendo una limpieza y primera exploración de los datos. Los datos incluyen características del empleado, si este abandonó o no la empresa y otros datos de satisfacción. 

Abandono por puesto:

![imagen](https://user-images.githubusercontent.com/87567925/229365803-aaabc298-6eac-4777-ada5-e0e79bc2b046.png)


Analizando al grupo de trabajadores que dejaron la empresa, hemos construido un perfil medio. 
* Bajo nivel educativo
* Soltero
* Trabaja en ventas
* Bajo salario
* Alta carga de horas extras

Así pues, los actuales empleados que más se acerquen a este perfil son los que estarán en un mayor riesgo de abandono.

### Segunda parte: impacto económico ([Notebook](https://github.com/adrianriverof/fuga-empleados/blob/main/2_impacto_economico.ipynb))

Con el fin de cuantificar el problema, y valorar mejor sobre qué grupo de empleados merece la pena priorizar, vamos a estimar las pérdidas que se estiman por cada empleado.
Siguiendo unas estimaciones de un estudio del Center for American Progress, la estimación nos dice que:
* en el último año las pérdidas por aband ono se estiman 2719005.91€
* las pérdidas de empleados que no estaban motivados fueron 368672.69€

Podemos estimar el ahorro que supondría retener a un porcentaje de estos empleados:
* 30% - 815701€
* 20% - 543801€
* 10% - 271900€

Hemos visto también que, sobre el grupo de mayor riesgo (representantes de ventas), retener un 30% (5 empleados) supondría un ahorro de 37447.22€

De este modo, podemos estimar un presupuesto para acciones de retención por cada departamento o perfil. 

### Tercera parte: modelo de machine learning ([Notebook](https://github.com/adrianriverof/fuga-empleados/blob/main/3_modelo_machine_learning%20.ipynb))

Ahora vamos a hacer uso de herramientas de machine learning para construir un modelo que pueda establecer una medida de cómo de probable es que un empleado de ciertas características vaya a abandonar la empresa.
Usando este modelo en un futuro, a partir de datos recolectados, se podrán prever casos de abandono y actuar de forma preventiva sobre ellos.

Gracias a esto podemos obtener información útil:

#### Importancia de las variables


![imp_var](https://user-images.githubusercontent.com/87567925/229366609-4d92bfb9-4017-4e6c-bb3f-152bf56c0a63.png)


#### Riesgo de abandono por puesto


![imagen](https://user-images.githubusercontent.com/87567925/229364988-3d4251ed-65fd-439f-90a8-726d7b3215e3.png "Riesgo de abandono por puesto")

#### Dashboard

Con el fin de facilitar la consulta de esta información, hemos elaborado un [dashboard interactivo en Tableau](https://public.tableau.com/app/profile/adrian.rivero8038/viz/PracticaDashboard_16628045185180/Dashboard1) en el que se puede consultar el porcentaje de fuga, la cantidad de empleados y el dinero perdido por departamento. 

![Dashboard general](https://user-images.githubusercontent.com/87567925/229365387-b23d9384-a127-4f11-9aca-ad19276e439d.png "Dashboard en Tableau")





