# Comenzando con ACUS220

## Distribución Anaconda y entorno virtual.

+ Muchas de las `aplicaciones` de Python requieren `paquetes` y `módulos` que no son parte de la `librería` estándar. 
+ Además, cualquiera aplicación necesitará una `versión` específica de una `librería`.
+ Qué significa ésto? Que podría ocurrir que no sea posible que una instalación de Python cumpla con los todos los requisitos de una aplicación. Por ejemplo, si la aplicación `acus_1` necesita la versión 1.0 de un módulo en particular, pero la aplicación `acus_2` necesita la versión 2.0, entonces los requisitos están en `conflicto de versiones` y la instalación de la versión 1.0, ó 2.0, dejará una aplicación `incapaz` de ejecutarse.
+ La solución para este problema de `conflicto de versiones` es crear un `entorno virtual`, esto es, se trata de un árbol de directorios, autocontenido que contenga una instalación de Python para una versión específica.
+ Distintas `aplicaciones` pueden utilizar diferentes entornos virtuales. Por ejemplo, para solucionar el conflicto anterior de requisitos, la aplicación `acus_1` puede tener su propio entorno virtual con la versión 1.0 instalada. Mientras que, la aplicación `acus_2` tiene otro entorno virtual con la versión 2.0 instalada. Además, en el caso hipotético que la aplicación `acus_2` pudiera requerir que una `librería` se actualice a la versión 3.0, `esto no afectará` el entorno de la aplicación `acus_1`.
+ Para sistema de administración de `paquetes` y un sistema de administración de `entornos virtuales` de `código abierto` que se ejecuta en Windows, macOS y Linux, ver [Conda](https://conda.io/projects/conda/en/latest/index.html), y para apoyar estos conceptos ver [Administración de ambientes](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).

## Manejador de paquetes Conda por medio de la instalación de Miniconda.
