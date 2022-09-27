# Comenzando con ACUS220

## Distribución Anaconda y entorno virtual.
+ ¿Por qué necesitamos configurar un entorno virtual?
+ Muchas de las `aplicaciones` de Python requieren `paquetes` y `módulos` que no son parte de la `librería` estándar. 
+ Además, cualquiera aplicación necesitará una `versión` específica de una `librería`.
+ Qué significa ésto? Que podría ocurrir que no sea posible que una instalación de Python cumpla con los todos los requisitos de una aplicación. Por ejemplo, si la aplicación `acus_1` necesita la versión 1.0 de un módulo en particular, pero la aplicación `acus_2` necesita la versión 2.0, entonces los requisitos están en `conflicto de versiones` y la instalación de la versión 1.0, ó 2.0, dejará una aplicación `incapaz` de ejecutarse.
+ La solución para este problema de `conflicto de versiones` es crear un `entorno virtual`, esto es, se trata de un árbol de directorios, autocontenido que contenga una instalación de Python para una versión específica.
+ Distintas `aplicaciones` pueden utilizar diferentes entornos virtuales. Por ejemplo, para solucionar el conflicto anterior de requisitos, la aplicación `acus_1` puede tener su propio entorno virtual con la versión 1.0 instalada. Mientras que, la aplicación `acus_2` tiene otro entorno virtual con la versión 2.0 instalada. Además, en el caso hipotético que la aplicación `acus_2` pudiera requerir que una `librería` se actualice a la versión 3.0, `esto no afectará` el entorno de la aplicación `acus_1`.
+ Anaconda ofrece la forma más fácil de usar Python en diversas aplicaciones, por ejemplo, en minería de datos, aprendizaje de máquinas, en una sola máquina. Podemos comenzar a trabajar con muchos paquetes y librerías de código abierto: Ver [Anaconda](https://www.anaconda.com/), y para apoyar estos conceptos ver [Administración de ambientes](https://www.anaconda.com/products/distribution).

## Manejador de paquetes Conda por medio de la instalación de Miniconda.
+ `Conda` es un sistema de gestión de entornos y paquetes de código abierto que se ejecuta en Windows, macOS y Linux. 
+ Conda instala, ejecuta y actualiza rápidamente los paquetes y sus dependencias. 
+ También crea, guarda, carga y cambia fácilmente entre entornos en nuestro computador local. Fue creado para programas de Python, pero puede empaquetar y distribuir software para cualquier idioma.
+ `Miniconda` es un instalador mínimo gratuito para `conda`. Es una pequeña versión de arranque de Anaconda que incluye sólo conda, Python, los paquetes de los que dependen y una pequeña cantidad de otros paquetes útiles, incluidos pip, zlib y algunos otros. 
+ Utilizamos [Mininaconda] https://docs.conda.io/en/latest/miniconda.html
