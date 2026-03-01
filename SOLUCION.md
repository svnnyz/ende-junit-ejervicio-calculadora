# PRUEBAS

**1. ¿Qué sentido puede tener este proyecto y para que lo podrías usar?**

_El objetivo de este proyecto es aprender sobre el funcionamiento de las pruebas en Junit con una calculadora sencilla, y la realización de pruebas de caja negra._ 

_Se podría usar como base para proyectos más grandes, que necesiten hacer cálculos_

**2. Revisa las pruebas de la suma y comenta lo que te parezca de interés**

_Es una prueba sin mayor complicación, escribir el código es fácil_
_Como adición, para que los resultados de las operaciones sean más exactos, se podría usar el tipo float en vez de int_
_También, es muy útil que te marque las pruebas que salieron mal, así se pueden corregir de forma simple y sin revisar cada parte del código._

**3. Realiza un estudio de caja negra de la división e implementa las pruebas en junit: Se realizará en markdown.**


RANGO VÁLIDO:
-infinito a 0
De 0 a infinito
RANGO INVÁLIDO 
Divisor 0

Se prueban los valores límite, los valores debajo y encima del límite y los valores medios entre rangos


| Caso de prueba| Clase de equivalencia |   Límite       |   Valor   |  Salida  |        
| --------------| --------------------- | ---------------| ----------|----------|
|     CP1       | Resultados válidos    |    -infinito   |    -800   | Resultado|
|     CP2       |                       |  valor medio   |    -400   | Resultado|
|     CP3       |                       |     < 0        |     -1    | Resultado|
|     CP4       |                       |     = 0        |      0    | Resultado|  
|     CP5       |                       |     > 0        |      1    | Resultado|
|     CP6       |                       | infinito       |     700   | Resultado|
|     CP7       | Resultados no válidos | divisor 0      |       0   |  error!  |


El código está a partir de la línea 37 en CalculadoraTest.java
