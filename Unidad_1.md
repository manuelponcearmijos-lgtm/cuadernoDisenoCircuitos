 <div align="center">

# ⚡ TRANSISTORES ⚡

### 🔌 Fundamentos · Funcionamiento · Aplicaciones

![Electrónica](https://img.shields.io/badge/ELECTRÓNICA-TRANSISTORES-00BFFF?style=for-the-badge)
![Circuitos](https://img.shields.io/badge/DISEÑO-CIRCUITOS-7B2CBF?style=for-the-badge)

</div>

---

## 🔋 1. ¿Qué es un transistor?

Un **transistor** es un componente semiconductor utilizado para amplificar señales eléctricas y funcionar como interruptor electrónico. Es fundamental en computadoras, teléfonos, sistemas de control y circuitos digitales.

<div align="center">

![Transistor electrónico](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Transistors.agr.jpg/640px-Transistors.agr.jpg)

*Figura 1. Diferentes tipos de transistores.*

</div>

## ⚙️ 2. Partes principales

En un transistor bipolar (BJT) encontramos tres terminales:

| Terminal | Función |
|---|---|
| **Base (B)** | Controla la conducción. |
| **Colector (C)** | Recibe la corriente principal en un NPN típico. |
| **Emisor (E)** | Permite la salida de la corriente en un NPN típico. |

## 🔌 3. Tipos de transistores

<div align="center">

| 🔵 Transistor NPN | 🟣 Transistor PNP |
|---|---|
| ![Transistor NPN](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1c/NPN_BJT.svg/220px-NPN_BJT.svg.png) | ![Transistor PNP](https://upload.wikimedia.org/wikipedia/commons/thumb/6/60/PNP_BJT.svg/220px-PNP_BJT.svg.png) |
| Conduce cuando la base tiene suficiente polarización positiva respecto al emisor. | Conduce cuando la base tiene suficiente polarización negativa respecto al emisor. |

</div>

**Otros tipos importantes:**

- 🔹 **MOSFET:** controlado por tensión, muy utilizado en electrónica digital.
- 🔹 **JFET:** transistor de efecto de campo empleado en circuitos electrónicos.
- 🔹 **BJT:** transistor bipolar usado en amplificación y conmutación.

## 💡 4. ¿Cómo funciona?

Un transistor puede trabajar principalmente en dos modos:

<details>
<summary><b>🟢 Modo de corte — Interruptor abierto</b></summary>

La corriente de control es insuficiente y el transistor permanece apagado, por lo que prácticamente no circula corriente entre colector y emisor en un BJT.

</details>

<details>
<summary><b>🔴 Modo de saturación — Interruptor cerrado</b></summary>

El transistor recibe suficiente corriente de base y permite que circule corriente entre colector y emisor, dentro de los límites del componente.

</details>

<details>
<summary><b>🔵 Modo activo — Amplificación</b></summary>

Una pequeña variación en la corriente de base puede controlar una variación mayor en la corriente del colector, permitiendo amplificar señales.

</details>

## 🧪 5. Diseño de un circuito con transistor

### 💡 Encendido de un LED mediante un transistor NPN

```text
           +V
            |
           [R2]
            |
           LED
            |
            C
Entrada─[R1]─B   Q1 (NPN)
            E
            |
           GND
```

**Componentes:**

- 🔋 Fuente de alimentación.
- ⚙️ Transistor NPN.
- 💡 LED.
- 🔧 Resistencias limitadoras.
- 🔌 Cables de conexión.

**Funcionamiento:** cuando la señal de entrada activa la base, el transistor conduce y permite encender el LED. Al retirar la señal, el LED se apaga si el transistor vuelve al corte.

> ⚠️ Los valores de las resistencias y la tensión de alimentación deben seleccionarse según el transistor y el LED utilizados.

## 🖥️ 6. Aplicaciones de los transistores

<div align="center">

| 💻 Computación | 🔊 Electrónica | 🤖 Automatización |
|---|---|---|
| Procesadores y memoria | Amplificadores de audio | Control de motores |
| Circuitos lógicos | Fuentes de alimentación | Sensores y actuadores |

</div>

## 🎯 Conclusión

Los transistores son componentes esenciales en el diseño de circuitos electrónicos porque permiten controlar la corriente, amplificar señales y realizar funciones de conmutación. Comprender sus terminales, tipos y modos de funcionamiento facilita el diseño de circuitos prácticos y sistemas digitales.

---

<div align="center">

**⚡ DISEÑAR · CONECTAR · SIMULAR · INNOVAR ⚡**

*Portafolio Digital — Diseño de Circuitos | Segundo Ciclo*

</div>

 <div align="center">

# ⚡ COMPUERTAS LÓGICAS Y SISTEMAS BINARIOS ⚡

### 💻 Diseño de Circuitos · Segundo Ciclo

![Electrónica digital](https://img.shields.io/badge/ELECTRÓNICA-DIGITAL-00BFFF?style=for-the-badge)
![Sistemas binarios](https://img.shields.io/badge/SISTEMAS-BINARIOS-7B2CBF?style=for-the-badge)
![Lógica](https://img.shields.io/badge/DISEÑO-COMPUERTAS_LÓGICAS-FF6600?style=for-the-badge)

</div>

---

## 🔢 1. Sistemas binarios

El **sistema binario** es un sistema de numeración de base 2 que utiliza únicamente los dígitos **0 y 1**. Es fundamental en las computadoras y los circuitos digitales, ya que permite representar y procesar información mediante señales eléctricas.

### 💡 Conversión de binario a decimal

Cada posición representa una potencia de 2, comenzando desde \(2^0\), de derecha a izquierda.

**Ejemplo:**

\[
1011_2 = 1(2^3)+0(2^2)+1(2^1)+1(2^0)
\]

\[
=8+0+2+1=\boxed{11_{10}}
\]

### 🔄 Tabla de equivalencias

| Decimal | Binario |
|:---:|:---:|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |
| 10 | 1010 |

**Operaciones binarias básicas:**

- **Suma:** \(0+0=0\), \(0+1=1\), \(1+1=10\).
- **Resta:** \(1-0=1\), \(1-1=0\).
- **Multiplicación:** \(1\times1=1\); cualquier número multiplicado por 0 da 0.

---

## ⚙️ 2. ¿Qué son las compuertas lógicas?

Las **compuertas lógicas** son componentes electrónicos que reciben una o más entradas binarias y producen una salida según una operación lógica. Son la base de los procesadores, las memorias y los sistemas digitales.

### 🔌 Principales compuertas lógicas

| Compuerta | Operación | ¿Cuándo da 1? |
|---|---|---|
| AND | \(A\cdot B\) | Cuando ambas entradas son 1. |
| OR | \(A+B\) | Cuando al menos una entrada es 1. |
| NOT | \(\overline{A}\) | Cuando la entrada es 0. |
| NAND | \(\overline{A\cdot B}\) | Cuando al menos una entrada es 0. |
| NOR | \(\overline{A+B}\) | Cuando ambas entradas son 0. |
| XOR | \(A\oplus B\) | Cuando las entradas son diferentes. |
| XNOR | \(\overline{A\oplus B}\) | Cuando las entradas son iguales. |

### 🧠 Tablas de verdad

La tabla de verdad muestra todas las combinaciones posibles de entradas y sus salidas.

**Compuertas de dos entradas:**

| A | B | AND | OR | NAND | NOR | XOR | XNOR |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| 0 | 0 | 0 | 0 | 1 | 1 | 0 | 1 |
| 0 | 1 | 0 | 1 | 1 | 0 | 1 | 0 |
| 1 | 0 | 0 | 1 | 1 | 0 | 1 | 0 |
| 1 | 1 | 1 | 1 | 0 | 0 | 0 | 1 |

**Compuerta NOT:**

| A | Salida |
|:---:|:---:|
| 0 | 1 |
| 1 | 0 |

---

## 🔬 3. Diseño de circuitos lógicos

Las compuertas pueden conectarse entre sí para construir circuitos que resuelven problemas mediante operaciones binarias.

### 💡 Ejemplo: circuito AND

```text
Entrada A ───┐
             ├── [ AND ] ─── Salida Y
Entrada B ───┘
```

Su expresión lógica es:

\[
Y=A\cdot B
\]

La salida será 1 solamente cuando las entradas A y B sean iguales a 1.

### 🚦 Ejemplo práctico: sistema de seguridad

Un sistema tiene dos sensores: A (puerta) y B (ventana). La alarma se activa únicamente cuando ambos sensores detectan una apertura.

\[
\text{Alarma}=A\cdot B
\]

Este ejemplo representa una condición lógica AND y puede implementarse mediante un circuito digital.

---

## 🛠️ 4. Aplicaciones en computación

- 💻 **Procesadores:** ejecutan operaciones lógicas y aritméticas.
- 🧠 **Memorias digitales:** almacenan información binaria.
- 🚨 **Sistemas de seguridad:** procesan señales de sensores.
- 🤖 **Automatización:** controlan máquinas y dispositivos.
- 🔌 **Circuitos combinacionales:** permiten diseñar sumadores, comparadores y otros sistemas digitales.

---

## 🎯 Conclusión

Los sistemas binarios permiten representar la información mediante ceros y unos, mientras que las compuertas lógicas procesan esos valores para producir resultados. Ambos conceptos son fundamentales para comprender el funcionamiento de los circuitos digitales y constituyen una base importante en la formación de Ingeniería en Computación.

---

<div align="center">

### ⚡ LÓGICA · BINARIO · DISEÑO DIGITAL ⚡

*Portafolio Digital — Diseño de Circuitos*

**Segundo Ciclo · Universidad Nacional de Loja**

</div>
