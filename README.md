# CalculoOfertaDiaria

# Cálculo de la Oferta de Forraje por Vaca por Día

https://josefernandoguarin.github.io/CalculoOfertaDiaria/

## Lógica del cálculo

El principio central es: **¿cuántos metros cuadrados de pradera tiene disponibles cada vaca cada día?** Una vez obtenido ese valor, basta multiplicarlo por el aforo para obtener la oferta en kilogramos de forraje fresco.

---

## Paso 1 — Rotaciones por año

$$\text{Rotaciones/año} = \frac{365 \text{ días}}{42 \text{ días de rotación}} = 8{,}69 \text{ rot/año}$$

Este valor indica cuántas veces al año se recorre el sistema de pastoreo completo.

---

## Paso 2 — Área total ofrecida por año

$$\text{Área ofrecida} = 64 \text{ ha} \times 8{,}69 \text{ rot/año} = 556 \text{ ha/año}$$

Se interpreta como la superficie acumulada que el sistema pone a disposición de los animales a lo largo del año.

---

## Paso 3 — Conversión a metros cuadrados

$$556 \text{ ha/año} \times 10.000 \text{ m}^2/\text{ha} = 5.560.000 \text{ m}^2/\text{año}$$

---

## Paso 4 — Área disponible por día

$$\frac{5.560.000 \text{ m}^2/\text{año}}{365 \text{ días}} = 15.233 \text{ m}^2/\text{día}$$

---

## Paso 5 — Área por vaca por día

$$\frac{15.233 \text{ m}^2/\text{día}}{N° \text{ vacas}} = \text{m}^2/\text{vaca/día}$$

> *Ejemplo: con 120 vacas → 15.233 / 120 = **127 m²/vaca/día***

---

## Paso 6 — Oferta de forraje por vaca por día

$$\text{m}^2/\text{vaca/día} \times \text{Aforo (kg FV/m}^2) = \text{kg FV/vaca/día}$$

> *Ejemplo: 127 m² × 2,5 kg FV/m² = **317 kg FV/vaca/día***

---

## Resumen en fórmula única

$$\text{Oferta (kg FV/vaca/día)} = \frac{\text{ha} \times \frac{365}{d_{rot}} \times 10.000}{365 \times N_{vacas}} \times \text{Aforo}$$

Que simplificada queda:

$$= \frac{\text{ha} \times 10.000}{d_{rot} \times N_{vacas}} \times \text{Aforo}$$

---

**Nota:** Este cálculo representa la **oferta potencial**. La oferta real depende además de la eficiencia de cosecha (pérdidas por pisoteo, rechazo y residuo post-pastoreo), que generalmente oscila entre 60–80 % en sistemas rotativos.
