---
description: >-
  La suma sigma de Riemann y los límites, que es donde reside el verdadero poder
  del concepto y nos lleva a la definición formal de la integral definida.
---

# Suma sigma de Riemann y los límites

#### **El Puente: Del aproximado al exacto**

La suma de Riemann por sí sola, Sn=∑i=1nf(ci) ΔxSn​=∑i=1n​f(ci​)Δx, es solo una **aproximación** del área bajo la curva. Su precisión depende completamente de dos factores:

1. El número de subintervalos $$n$$
2. La elección del punto muestral  $$c_{i}$$&#x20;

Para obtener el valor **exacto** del área, necesitamos refinar esta aproximación al máximo. Aquí es donde entran los límites.

***

#### **La definición formal de la integral definida**

La integral definida de una función $$f(x)$$ sobre el intervalo  $$[a,b]$$ se define como el **límite** de su suma de Riemann cuando el número de subintervalos tiende a infinito   $$n-> /infinity$$ .

$$∫_0^2x^2 dx=\frac{8}{3}$$$$∫abf(x) dx=lim⁡n→∞∑i=1nf(ci) Δx∫ab​f(x)dx=n→∞lim​i=1∑n​f(ci​)Δx$$∫abf(x) dx=lim⁡n→∞∑i=1nf(ci) Δx∫ab​f(x)dx=n→∞lim​i=1∑n​f(ci​)Δx

$$∫_0^2x^2 dx=\frac{8}{3}$$

**¿Qué significa esto?**

* $$∫_0^2x^2 dx=\frac{8}{3}$$**n→∞n→∞**: Imaginamos dividir el intervalo \[a,b]\[a,b] en un número infinitamente grande de subintervalos.
* $$∫_0^2x^2 dx=\frac{8}{3}$$**Δx→0Δx→0**: Como Δx=b−anΔx=nb−a​, si `n` se hace infinitamente grande, el ancho de cada rectángulo se vuelve infinitesimalmente pequeño $$∫_0^2x^2 dx=\frac{8}{3}$$(Δx→0Δx→0).
* **El límite existe**: Si este límite da un valor único y finito, independientemente de cómo elijamos los puntos muestrales cici​, decimos que la función ff es **integrable** en $$∫_0^2x^2 dx=\frac{8}{3}$$\[a,b]\[a,b].

Al tomar este límite, la suma de áreas de rectángulos (que es una aproximación) se convierte en la suma exacta de un número infinito de áreas infinitesimales, que es el área bajo la curva.

***

#### **Proceso Paso a Paso: De la Suma al Límite**

Veamos este proceso con un ejemplo concreto.

**Problema:** Calcular el **valor exacto** de $$∫_0^2x^2 dx=\frac{8}{3}$$∫02x2 dx∫02​x2dx usando la definición de límite de una suma de Riemann.

**Paso 1: Establecer la suma para `n` subintervalos.**

* $$∫_0^2x^2 dx=\frac{8}{3}$$a=0a=0, b=2b=2
* $$∫_0^2x^2 dx=\frac{8}{3}$$Δx=b−an=2−0n=2nΔx=nb−a​=n2−0​=n2​
*   Elegimos usar el **extremo derecho** para los puntos muestrales (es más fácil para este cálculo). El punto final del i-ésimo subintervalo es:

    $$∫_0^2x^2 dx=\frac{8}{3}$$xi=a+i⋅Δx=0+i⋅2n=2inxi​=a+i⋅Δx=0+i⋅n2​=n2i​

    Por lo tanto, $$∫_0^2x^2 dx=\frac{8}{3}$$ci=xi=2inci​=xi​=n2i​.

**Paso 2: Escribir la suma de Riemann** $$S_{n}$$**​.**

$$∫_0^2x^2 dx=\frac{8}{3}$$Sn=∑i=1nf(ci) Δx=∑i=1nf(2in)⋅2nSn​=i=1∑n​f(ci​)Δx=i=1∑n​f(n2i​)⋅n2​

Como f(x)=x2f(x)=x2, entonces f(2in)=(2in)2=4i2n2f(n2i​)=(n2i​)2=n24i2​. Sustituyendo:

$$Sn=∑i=1n(4i2n2)⋅2n=∑i=1n8i2n3Sn​=i=1∑n​(n24i2​)⋅n2​=i=1∑n​n38i2​$$

**Paso 3: Simplificar la sumatoria.**\
Podemos sacar las constantes (8n3n38​) fuera de la sumatoria:

$$Sn=8n3∑i=1ni2Sn​=n38​i=1∑n​i2$$

Existe una fórmula para la suma de los primeros `n` cuadrados:

$$∑i=1ni2=n(n+1)(2n+1)6i=1∑n​i2=6n(n+1)(2n+1)​$$

Sustituyendo esta fórmula:

$$Sn=8n3⋅n(n+1)(2n+1)6=8n(n+1)(2n+1)6n3=4(n+1)(2n+1)3n2Sn​=n38​⋅6n(n+1)(2n+1)​=6n38n(n+1)(2n+1)​=3n24(n+1)(2n+1)​$$&#x20;

(Simplificamos $$∫_0^2x^2 dx=\frac{8}{3}$$86=4368​=34​ y n/n3=1/n2n/n3=1/n2).

**Paso 4: Tomar el límite cuando n→∞n→∞.**\
La integral es el límite de esta expresión simplificada:

$$∫02x2 dx=lim⁡n→∞Sn=lim⁡n→∞[4(n+1)(2n+1)3n2]∫02​x2dx=n→∞lim​Sn​=n→∞lim​[3n24(n+1)(2n+1)​]$$

**Paso 5: Evaluar el límite.**\
Para evaluar&#x20;

$$\lim⁡_{n\rightarrow\infty}\frac{4(n+1)(2n+1)}{3n^2}$$, expandimos el numerador y dividimos cada término por n2n2:

$$\frac{4(n+1)(2n+1)}{3n^2}=\frac{4(2n2+3n+1)}{3n^2}=\frac{8n^2+12n+4}{3n^2}=\frac{8}{3}+\frac{12}{3n}+\frac{4}{3n^2}$$

Ahora tomamos el límite:

$$\lim⁡_{n\rightarrow\infty}(\frac{8}{3}+\frac{12}{3n}+\frac{4}{3n^2})=\frac{8}{3}+0+0=\frac{8}{3}$$

**Resultado final:**

$$∫_0^2x^2 dx=\frac{8}{3}$$

***

#### **Interpretación y conclusión**

* **Aproximación vs. realidad:** Si recuerdas el primer ejercicio $$n= número$$, las aproximaciones oscilaban. Al usar el límite, encontramos el valor exacto.
* **El poder del límite:** El proceso de límite **elimina el error** inherente a la aproximación. No importa si usamos extremos derechos, izquierdos o puntos medios; el límite siempre convergerá al mismo valor para funciones integrables.
* **Notación:** La notación de integral$$\int$$ es una "S" alargada, elegida específicamente por Leibniz para representar la "suma" infinita (Summa) de estas áreas infinitesimales.
