# Sumas de Riemann

### Historia

Las **sumas de Riemann** llevan el nombre del matemático alemán **Bernhard Riemann** (1826-1866), quien las desarrolló en el siglo XIX como parte de su trabajo sobre la teoría de la integración. Riemann presentó estas ideas en su trabajo "Sobre la representación de una función mediante una serie trigonométrica" (1854), donde formalizó el concepto de integral definida mediante límites de sumas.

Aunque el concepto de aproximar áreas bajo curvas era conocido desde la antigüedad (Arquímedes usó métodos similares), Riemann proporcionó la primera definición rigurosa de la integral definida, sentando las bases del cálculo integral moderno.

### Definición

Las sumas de Riemann son aproximaciones del área bajo una curva (integral definida) mediante la suma de áreas de rectángulos. Dada una función f(x)f(x) definida en un intervalo \[a,b]\[a,b], se divide el intervalo en nn subintervalos de ancho Δx=b−anΔx=nb−a​.

La suma de Riemann se define como:

Sn=∑i=1nf(xi∗)ΔxSn​=i=1∑n​f(xi∗​)Δx

donde xi∗xi∗​ es un punto cualquiera en el i-ésimo subintervalo \[xi−1,xi]\[xi−1​,xi​].

### Tipos de sumas de Riemann

#### 1. Suma por la izquierda

Se toma el valor de la función en el extremo izquierdo de cada subintervalo:

xi∗=xi−1xi∗​=xi−1​

#### 2. Suma por la derecha

Se toma el valor de la función en el extremo derecho de cada subintervalo:

xi∗=xixi∗​=xi​

#### 3. Suma por el punto medio

Se toma el valor de la función en el punto medio de cada subintervalo:

xi∗=xi−1+xi2xi∗​=2xi−1​+xi​​

**La Notación Sigma (Σ) en las Sumas de Riemann**

La notación sigma (Σ) es una forma compacta y elegante de representar una suma de muchos términos. En el contexto de las sumas de Riemann, nos permite expresar de manera precisa la idea de sumar las áreas de todos los rectángulos que aproximan el área bajo una curva.

**1. Desglose de la Fórmula**

La suma de Riemann para una función f(x)f(x) en el intervalo \[a,b]\[a,b], dividido en nn subintervalos, se escribe como:

Sn=∑i=1nf(ci) ΔxSn​=i=1∑n​f(ci​)Δx

Donde:

* **∑∑ (Sigma)**: El símbolo de sumatoria. Indica que debemos sumar una serie de términos.
* **i=1i=1 (índice inferior)**: El punto de partida del contador de la suma. Nos dice que el primer rectángulo a considerar es el número 1.
* **nn (índice superior)**: El punto final del contador. Nos dice que el último rectángulo a considerar es el número nn. La suma incluirá nn términos.
* **f(ci)f(ci​)**: La altura del i-ésimo rectángulo. Es el valor de la función evaluada en un punto muestral cici​ dentro del i-ésimo subintervalo.
* **ΔxΔx**: El ancho de la base de cada rectángulo. Se calcula como Δx=b−anΔx=nb−a​. Como es constante para todos los rectángulos, se puede factorizar fuera de la sumatoria.

**2. Cómo Funciona la Notación**

La expresión ∑i=1nf(ci) Δx∑i=1n​f(ci​)Δx es una instrucción que significa:

> "Para ii igual a 1, luego 2, luego 3, y así sucesivamente hasta llegar a nn, toma el valor de f(ci) Δxf(ci​)Δx, y suma todos estos valores juntos."

En otras palabras:

Sn=f(c1)Δx+f(c2)Δx+f(c3)Δx+…+f(cn)ΔxSn​=f(c1​)Δx+f(c2​)Δx+f(c3​)Δx+…+f(cn​)Δx

**3. Ejemplo Práctico con Notación Sigma**

**Problema:** Aproximar ∫13(x2+1) dx∫13​(x2+1)dx usando una suma de Riemann por la **derecha** con n=4n=4 subintervalos.

**Paso 1: Calcular ΔxΔx**

Δx=b−an=3−14=24=0.5Δx=nb−a​=43−1​=42​=0.5

**Paso 2: Identificar los puntos y los puntos muestrales cici​ (elegimos el extremo derecho)**\
Los subintervalos son:

* \[1.0,1.5]\[1.0,1.5]
* \[1.5,2.0]\[1.5,2.0]
* \[2.0,2.5]\[2.0,2.5]
* \[2.5,3.0]\[2.5,3.0]

Los puntos muestrales para la suma por la derecha son:\
c1=1.5c1​=1.5, c2=2.0c2​=2.0, c3=2.5c3​=2.5, c4=3.0c4​=3.0

**Paso 3: Escribir la Suma de Riemann con Notación Sigma**

S4=∑i=14f(ci) Δx=Δx ∑i=14f(ci)S4​=i=1∑4​f(ci​)Δx=Δxi=1∑4​f(ci​)S4=0.5 \[f(1.5)+f(2.0)+f(2.5)+f(3.0)]S4​=0.5\[f(1.5)+f(2.0)+f(2.5)+f(3.0)]

**Paso 4: Calcular los valores de la función (f(x)=x2+1f(x)=x2+1)**

* f(1.5)=(1.5)2+1=2.25+1=3.25f(1.5)=(1.5)2+1=2.25+1=3.25
* f(2.0)=(2.0)2+1=4+1=5f(2.0)=(2.0)2+1=4+1=5
* f(2.5)=(2.5)2+1=6.25+1=7.25f(2.5)=(2.5)2+1=6.25+1=7.25
* f(3.0)=(3.0)2+1=9+1=10f(3.0)=(3.0)2+1=9+1=10

**Paso 5: Sustituir y resolver**

S4=0.5 \[3.25+5+7.25+10]=0.5 \[25.5]=12.75S4​=0.5\[3.25+5+7.25+10]=0.5\[25.5]=12.75

**Interpretación:** La suma de las áreas de los 4 rectángulos (definidos por los extremos derechos) es 12.75, que es una aproximación del área bajo la curva f(x)=x2+1f(x)=x2+1 entre x=1x=1 y x=3x=3.

#### **Resumen de los Tipos de Suma con Notación Sigma**

| Tipo de Suma           | Punto Muestral cici​                    | Fórmula con Notación Sigma                       |
| ---------------------- | --------------------------------------- | ------------------------------------------------ |
| **Por la izquierda**   | Extremo izquierdo: ci=xi−1ci​=xi−1​     | Sn=∑i=1nf(xi−1) ΔxSn​=∑i=1n​f(xi−1​)Δx           |
| **Por la derecha**     | Extremo derecho: ci=xici​=xi​           | Sn=∑i=1nf(xi) ΔxSn​=∑i=1n​f(xi​)Δx               |
| **Por el punto medio** | Punto medio: ci=xi−1+xi2ci​=2xi−1​+xi​​ | Sn=∑i=1nf(xi−1+xi2) ΔxSn​=∑i=1n​f(2xi−1​+xi​​)Δx |

En conclusión, la **notación sigma (Σ)** es la herramienta fundamental que nos permite expresar de manera concisa el proceso de sumar un número finito de términos para aproximar un área, sentando las bases para la definición formal de la integral definida.

\
