<div align="center">

# ⚡ COMPUERTAS LÓGICAS Y SISTEMAS BINARIOS ⚡

### 💻 Unidad 3 · Diseño de Circuitos · Segundo Ciclo

![Electrónica digital](https://img.shields.io/badge/ELECTRÓNICA-DIGITAL-00BFFF?style=for-the-badge)
![Sistemas binarios](https://img.shields.io/badge/SISTEMAS-BINARIOS-7B2CBF?style=for-the-badge)
![Lógica](https://img.shields.io/badge/DISEÑO-COMPUERTAS_LÓGICAS-FF6600?style=for-the-badge)

</div>

---

## 🔢 1. Sistemas binarios

El **sistema binario** es un sistema de numeración de base 2 que utiliza únicamente los dígitos **0 y 1**. Es fundamental en las computadoras y los circuitos digitales, ya que permite representar y procesar información mediante señales eléctricas.

### 💡 Conversión de binario a decimal

Cada posición representa una potencia de 2, comenzando desde $2^0$, de derecha a izquierda.

**Ejemplo:**

$$1011_2 = 1(2^3)+0(2^2)+1(2^1)+1(2^0)$$

$$= 8+0+2+1 = 11_{10}$$

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

- **Suma:** $0+0=0$, $0+1=1$, $1+1=10$ (se escribe 0 y se lleva 1).
- **Resta:** $0-0=0$, $1-0=1$, $1-1=0$, $0-1=1$ (pidiendo prestado 1 a la posición siguiente).
- **Multiplicación:** $1\times1=1$; cualquier número multiplicado por 0 da 0.

---

## ⚙️ 2. ¿Qué son las compuertas lógicas?

Las **compuertas lógicas** son componentes electrónicos que reciben una o más entradas binarias y producen una salida según una operación lógica. Son la base de los procesadores, las memorias y los sistemas digitales.

### 🔌 Principales compuertas lógicas

| Compuerta | Operación | ¿Cuándo da 1? |
|---|---|---|
| AND | $A\cdot B$ | Cuando ambas entradas son 1. |
| OR | $A+B$ | Cuando al menos una entrada es 1. |
| NOT | $\overline{A}$ | Cuando la entrada es 0. |
| NAND | $\overline{A\cdot B}$ | Cuando al menos una entrada es 0. |
| NOR | $\overline{A+B}$ | Cuando ambas entradas son 0. |
| XOR | $A\oplus B$ | Cuando las entradas son diferentes. |
| XNOR | $\overline{A\oplus B}$ | Cuando las entradas son iguales. |

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

$$Y=A\cdot B$$

La salida será 1 solamente cuando las entradas A y B sean iguales a 1.

### 🚦 Ejemplo práctico: sistema de seguridad

Un sistema tiene dos sensores: A (puerta) y B (ventana). La alarma se activa únicamente cuando ambos sensores detectan una apertura.

$$\text{Alarma}=A\cdot B$$

Este ejemplo representa una condición lógica AND y puede implementarse mediante un circuito digital.

---

## 🛠️ 4. Aplicaciones en computación

- 💻 **Procesadores:** ejecutan operaciones lógicas y aritméticas.
- 🧠 **Memorias digitales:** almacenan información binaria.
- 🚨 **Sistemas de seguridad:** procesan señales de sensores.
- 🤖 **Automatización:** controlan máquinas y dispositivos.
- 🔌 **Circuitos combinacionales:** permiten diseñar sumadores, comparadores y otros sistemas digitales.

---

## 🚧 Temas en desarrollo

- 🧩 Álgebra de Boole y simplificación de expresiones.
- 🔗 Circuitos combinacionales.
- 🖥️ Diseño y simulación digital.

> 📌 *Pendiente de completar:* capturas de simulación y proyecto práctico.

## 🎯 Conclusión

Los sistemas binarios permiten representar la información mediante ceros y unos, mientras que las compuertas lógicas procesan esos valores para producir resultados. Ambos conceptos son fundamentales para comprender el funcionamiento de los circuitos digitales y constituyen una base importante en la formación de Ingeniería en Computación.

---

<div align="center">

### ⚡ LÓGICA · BINARIO · DISEÑO DIGITAL ⚡

*Portafolio Digital — Diseño de Circuitos*

**Segundo Ciclo · Universidad Nacional de Loja**

[🏠 Inicio](./README.md) · [📘 Portada](./Portada.md) · [⬅️ Unidad 2](./Unidad_2.md)

</div>
