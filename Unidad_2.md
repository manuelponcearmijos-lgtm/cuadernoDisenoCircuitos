<div align="center">

# ⚡ ANÁLISIS Y DISEÑO DE CIRCUITOS ⚡

### 🔌 Unidad 2 · Diseño de Circuitos · Segundo Ciclo

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

**Familias principales:**

- 🔹 **BJT** (bipolar): controlado por corriente; usado en amplificación y conmutación. Es el que se estudia en esta unidad.
- 🔹 **MOSFET:** controlado por tensión, muy utilizado en electrónica digital.
- 🔹 **JFET:** transistor de efecto de campo empleado en circuitos electrónicos.

## 💡 4. ¿Cómo funciona?

Un transistor BJT puede trabajar en tres regiones:

<details>
<summary><b>🟢 Región de corte — Interruptor abierto</b></summary>

La corriente de base es insuficiente y el transistor permanece apagado, por lo que prácticamente no circula corriente entre colector y emisor.

</details>

<details>
<summary><b>🔴 Región de saturación — Interruptor cerrado</b></summary>

El transistor recibe suficiente corriente de base y permite que circule corriente entre colector y emisor, dentro de los límites del componente.

</details>

<details>
<summary><b>🔵 Región activa — Amplificación</b></summary>

Una pequeña variación en la corriente de base controla una variación mayor en la corriente del colector, lo que permite amplificar señales:

$$I_C = \beta \cdot I_B$$

</details>

Como interruptor, el transistor trabaja entre **corte** y **saturación**; como amplificador, en la **región activa**.

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

**Funcionamiento:** cuando la señal de entrada activa la base, el transistor conduce y permite encender el LED. Al retirar la señal, el LED se apaga porque el transistor vuelve al corte.

### 🧮 Cálculo de las resistencias

**Datos de ejemplo** (valores supuestos; deben ajustarse al transistor y LED reales):

| Dato | Valor |
|---|---|
| Alimentación y señal de entrada | $V = V_{in} = 5\ \text{V}$ |
| Caída del LED rojo | $V_{LED} \approx 2\ \text{V}$ |
| Corriente deseada en el LED | $I_C = 10\ \text{mA}$ |
| Saturación del transistor | $V_{CE(sat)} \approx 0{,}2\ \text{V}$ |
| Polarización base-emisor | $V_{BE} \approx 0{,}7\ \text{V}$ |
| Ganancia mínima (por ejemplo, 2N2222 o 2N3904) | $\beta \geq 100$ |

**Resistencia del LED (R2):**

$$R_2 = \frac{V - V_{LED} - V_{CE(sat)}}{I_C} = \frac{5 - 2 - 0{,}2}{0{,}010} = 280\ \Omega \;\Rightarrow\; 330\ \Omega\ \text{(comercial)}$$

**Resistencia de base (R1):** para asegurar la saturación se usa una ganancia forzada $\beta_f = 10$, menor que la real:

$$I_B = \frac{I_C}{\beta_f} = \frac{10\ \text{mA}}{10} = 1\ \text{mA}$$

$$R_1 = \frac{V_{in} - V_{BE}}{I_B} = \frac{5 - 0{,}7}{0{,}001} = 4{,}3\ \text{k}\Omega \;\Rightarrow\; 4{,}7\ \text{k}\Omega\ \text{(comercial)}$$

Con los valores comerciales, la corriente real del LED es de aproximadamente $\frac{5 - 2 - 0{,}2}{330} \approx 8{,}5\ \text{mA}$ y la de base de $\frac{4{,}3}{4700} \approx 0{,}9\ \text{mA}$, suficiente para saturar el transistor.

> ⚠️ Los valores de las resistencias y la tensión de alimentación deben seleccionarse según el transistor y el LED utilizados.

## 🖥️ 6. Aplicaciones de los transistores

<div align="center">

| 💻 Computación | 🔊 Electrónica | 🤖 Automatización |
|---|---|---|
| Procesadores y memoria | Amplificadores de audio | Control de motores |
| Circuitos lógicos | Fuentes de alimentación | Sensores y actuadores |

</div>

---

## 🚧 Temas en desarrollo

- 🔧 Circuitos en serie y paralelo.
- 📏 Leyes de Kirchhoff.
- 💻 Simulación de circuitos y comparación entre valores calculados y simulados.

> 📌 *Pendiente de completar:* capturas de simulación del circuito con transistor y análisis de resultados.

## 🎯 Conclusión

Los transistores son componentes esenciales en el diseño de circuitos electrónicos porque permiten controlar la corriente, amplificar señales y realizar funciones de conmutación. Comprender sus terminales, tipos y regiones de funcionamiento facilita el diseño de circuitos prácticos y sistemas digitales.

---

<div align="center">

**⚡ DISEÑAR · CONECTAR · SIMULAR · INNOVAR ⚡**

*Portafolio Digital — Diseño de Circuitos | Segundo Ciclo*

[🏠 Inicio](./README.md) · [📘 Portada](./Portada.md) · [⬅️ Unidad 1](./Unidad_1.md) · [➡️ Unidad 3](./Unidad_3.md)

</div>
