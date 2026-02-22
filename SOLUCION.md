# PRUEBAS

**1. ¿Qué sentido puede tener este proyecto y para que lo podrías usar?**

_Es una calculadora, es útil para realizar operaciones aritméticas en un instante._

**2. Revisa las pruebas de la suma y comenta lo que te parezca de interés**

_Es una prueba sin mayor complicación, escribir el código es fácil_

**3. Realiza un estudio de caja negra de la división e implementa las pruebas en junit: Se realizará en markdown.**


| Caso de prueba| Clase de equivalencia | prefijo |   entrada      | Tipo               |  Salida     | 
| --------------| --------------------- | ------- | ---------------| -------------------| ----------- | 
|     CP1       | Resultados válidos    | CErv    |    100/50      | entero positivo    |   2         |
|     CP2       |                       | CErv    | -70/-7         | ambos negativos    |   10        |
|     CP3       |                       | CErv    | -100/50        | signos distintos   |   -2        |
|     CP4       |  Resultados inválidos | CEri    |     4/0        |    divisor cero    |   Error     |


El código está a partir de la línea 37 en CalculadoraTest.java

((        @Test
    void dividir() {

        assertAll("division",
                () -> assertEquals(2, Calculadora.dividir(100, 50), "100 / 50 = 2"),
                () -> assertEquals(10, Calculadora.dividir(-70, -7), "(-70) / (-7) = 10"),
                () -> assertEquals(-2, Calculadora.dividir(-100, 50), "(-100) / 50 = (-2)"));
    }
))