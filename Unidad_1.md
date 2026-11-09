<div align="center">

# ⚡ FUNDAMENTOS DE ELECTRICIDAD Y ELECTRÓNICA ⚡

### 🔋 Unidad 1 · Diseño de Circuitos · Segundo Ciclo

![Electrónica](https://img.shields.io/badge/ELECTRÓNICA-FUNDAMENTOS-00BFFF?style=for-the-badge)
![Unidad](https://img.shields.io/badge/UNIDAD-1-0078D4?style=for-the-badge)

</div>

---

## ⚡ 1. Magnitudes eléctricas

| Magnitud | Símbolo | Unidad | Descripción |
|---|:---:|:---:|---|
| Voltaje (tensión) | $V$ | Voltio (V) | Diferencia de potencial que impulsa a las cargas por el circuito. |
| Corriente | $I$ | Amperio (A) | Cantidad de carga que circula por un punto en un segundo. |
| Resistencia | $R$ | Ohmio (Ω) | Oposición que ofrece un material al paso de la corriente. |
| Potencia | $P$ | Vatio (W) | Energía entregada o consumida por unidad de tiempo. |

La potencia se calcula como:

$$P = V \cdot I$$

---

## 📐 2. Ley de Ohm

La corriente que circula por un conductor es directamente proporcional al voltaje aplicado e inversamente proporcional a su resistencia:

$$V = I \cdot R \qquad I = \frac{V}{R} \qquad R = \frac{V}{I}$$

Combinando con la fórmula de potencia se obtiene también:

$$P = I^2 R = \frac{V^2}{R}$$

### 💡 Ejemplo

Una resistencia de $220\ \Omega$ se conecta a una fuente de $9\ \text{V}$:

$$I = \frac{9}{220} \approx 0{,}041\ \text{A} = 41\ \text{mA}$$

$$P = V \cdot I = 9 \times 0{,}041 \approx 0{,}37\ \text{W}$$

> ⚠️ Con $0{,}37\ \text{W}$ una resistencia común de $\tfrac{1}{4}\ \text{W}$ se sobrecalentaría. Por eso, además del valor óhmico, hay que verificar la potencia que soporta el componente.

---

## 🔌 3. Componentes electrónicos básicos

| Componente | Función | Detalle clave |
|---|---|---|
| **Resistencia** | Limita la corriente y divide tensiones. | Se identifica por su código de colores y su potencia nominal. |
| **Condensador** | Almacena energía en un campo eléctrico. | Se mide en faradios (F); los electrolíticos tienen polaridad. |
| **Diodo** | Permite el paso de corriente en un solo sentido. | Conduce en polarización directa (≈ 0,7 V en silicio). |
| **LED** | Diodo que emite luz al conducir. | Necesita resistencia limitadora en serie. |

### 💡 Resistencia limitadora para un LED

$$R = \frac{V_{fuente} - V_{LED}}{I_{LED}}$$

Con una fuente de $5\ \text{V}$, un LED rojo ($V_{LED} \approx 2\ \text{V}$) y $I_{LED} = 10\ \text{mA}$:

$$R = \frac{5 - 2}{0{,}010} = 300\ \Omega \;\Rightarrow\; \text{se usa el valor comercial de } 330\ \Omega$$

---

## 🔋 4. Fuentes de alimentación

- **Corriente continua (CC):** el voltaje mantiene siempre la misma polaridad (pilas, baterías, fuentes reguladas).
- **Corriente alterna (CA):** el voltaje cambia de polaridad periódicamente (red eléctrica domiciliaria).
- **Fuente ideal:** mantiene su voltaje sin importar la carga.
- **Fuente real:** tiene resistencia interna y su voltaje cae al aumentar la corriente demandada.

---

## 🧪 5. Instrumentos de medición: el multímetro

| Medición | Conexión del instrumento | Precaución |
|---|---|---|
| **Voltaje** | En **paralelo** con el elemento. | Seleccionar CC o CA según corresponda. |
| **Corriente** | En **serie** (se abre el circuito). | Nunca conectar en paralelo: puede dañar el equipo. |
| **Resistencia** | En paralelo, con el circuito **sin alimentación**. | Retirar el componente o desconectar la fuente. |

---

## 📊 6. Simbología electrónica

```text
Resistencia      Condensador      Diodo          LED            Fuente CC
  ─/\/\/─          ─┤├─           ─▶|─          ─▶|─ ↗↗         ─┤|├─
```

Interpretar correctamente los símbolos permite leer esquemas y reproducirlos luego en un simulador o en un montaje real.

---

## 🧾 Evidencias

> 📌 *Pendiente de completar:* capturas de simulación del circuito del LED, fotografías de mediciones con multímetro y comparación entre valores calculados y medidos.

---

## 🎯 Conclusión

La Unidad 1 establece las bases para el resto de la asignatura: las magnitudes eléctricas, la Ley de Ohm y el reconocimiento de los componentes y la simbología permiten calcular y verificar circuitos sencillos, como la resistencia limitadora de un LED. Estas bases se aplican en la Unidad 2 al analizar y diseñar circuitos más completos.

---

<div align="center">

**⚡ DISEÑAR · CONECTAR · SIMULAR · INNOVAR ⚡**

*Portafolio Digital — Diseño de Circuitos | Segundo Ciclo*

[🏠 Inicio](./README.md) · [📘 Portada](./Portada.md) · [➡️ Unidad 2](./Unidad_2.md)

</div>
