---
description: >-
  Los polígonos inscritos y circunscritos son un concepto fundamental en
  geometría y están directamente relacionados con las sumas de Riemann y el
  cálculo de áreas bajo curvas.
---

# Área debajo de la curva

### **Polígonos inscritos y circunscritos en el cálculo de áreas**

#### **1. Concepto geométrico**

* **Polígono inscrito**: Está dentro de una curva o círculo, con todos sus vértices tocando la curva.
* **Polígono circunscrito:** Rodea una curva o círculo, con todos sus lados tocando la curva.

#### **2. Relación con las sumas de Riemann**

En el contexto del cálculo integral, estos conceptos se aplican para aproximar el **área bajo una curva** ( y = f(x)):

* **Polígonos inscritos**: Corresponden a las **sumas inferiores de Riemann** (se usan rectángulos cuya altura es el mínimo de la función en cada subintervalo).
* **Polígonos circunscritos**: Corresponden a las **sumas superiores de Riemann** (se usan rectángulos cuya altura es el máximo de la función en cada subintervalo).

#### **3. Ejemplo con una función cóncava**

Consideremos $$f(x) = x^2 ) en ([0, 2])$$:

* **Polígonos inscritos (suma inferior)**:
  * Se elige el valor mínimo de f(x) en cada subintervalo (extremo izquierdo).
  * El área total es una **subestimación** del área real.
* **Polígonos circunscritos (suma superior)**:
  * Se elige el valor máximo de f(x)  en cada subintervalo (extremo derecho).
  * El área total es una **sobrestimación** del área real.

#### **4. Visualización**

* A medida que aumenta el número de subintervalos (( n \to \infty )):
  * Los polígonos inscritos y circunscritos se "ajustan" cada vez más a la curva.
  * Las sumas inferior y superior convergen al mismo valor: el área exacta bajo la curva.

#### **5. Teorema Fundamental**

Si ( f ) es continua en (\[a, b]), entonces: \[ \lim\_{n \to \infty} (\text{Suma inferior}) = \lim\_{n \to \infty} (\text{Suma superior}) = \int\_a^b f(x) , dx ] Esto garantiza que el área exacta puede aproximarse con precisión arbitraria usando polígonos inscritos o circunscritos.

***

### **Ejemplo concreto: ( \int\_0^2 x^2 , dx )**

#### **Para ( n = 4 ) subintervalos**:

* ( \Delta x = 0.5 ).
* **Suma inferior (inscrita)**:
  * Puntos: ( x = 0, 0.5, 1, 1.5 ).
  * Área = ( 0 \cdot 0.5 + 0.25 \cdot 0.5 + 1 \cdot 0.5 + 2.25 \cdot 0.5 = 1.75 ).
* **Suma superior (circunscrita)**:
  * Puntos: ( x = 0.5, 1, 1.5, 2 ).
  * Área = ( 0.25 \cdot 0.5 + 1 \cdot 0.5 + 2.25 \cdot 0.5 + 4 \cdot 0.5 = 3.75 ).

#### **Límite cuando ( n \to \infty )**:

* El valor real es ( \frac{8}{3} \approx 2.666... ), que está entre 1.75 y 3.75.
* Al aumentar ( n ), ambas sumas se acercan a ( \frac{8}{3} ).

***

### **Aplicaciones**

1. **Cálculo de áreas**: Aproximar áreas bajo curvas irregulares.
2. **Arquitectura y diseño**: Estimar áreas y volúmenes con formas complejas.
3. **Análisis numérico**: Métodos de integración numérica (regla del trapecio, regla de Simpson).

***

### **Ejercicio Propuesto**

Para ( f(x) = \sqrt{x} ) en (\[0, 4]):

1. Calcula la suma inferior y superior con ( n = 4 ).
2. Grafica los polígonos inscritos y circunscritos.
3. Verifica que el área real (( \frac{16}{3} )) esté entre ambas sumas.

**Solución**:

* ( \Delta x = 1 ).
* Suma inferior: ( f(0) + f(1) + f(2) + f(3) = 0 + 1 + \sqrt{2} + \sqrt{3} \approx 4.146 ).
* Suma superior: ( f(1) + f(2) + f(3) + f(4) = 1 + \sqrt{2} + \sqrt{3} + 2 \approx 6.146 ).
* Área real: ( \int\_0^4 \sqrt{x} , dx = \frac{16}{3} \approx 5.333 ).

***

#### **Conclusión**

Los polígonos inscritos y circunscritos son la base geométrica de las sumas de Riemann, permitiendo entender cómo se aproxima el área bajo una curva mediante procesos de límite. ¡Son esenciales para visualizar la integración!
