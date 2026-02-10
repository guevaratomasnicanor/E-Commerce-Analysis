# 🛒 Análisis de E-Commerce — Olist Marketplace (Brasil)

## 📌 Descripción del Proyecto
Este proyecto presenta un **análisis integral de Olist**, uno de los marketplaces de e-commerce más grandes de Brasil.  
El objetivo principal es **entender los drivers de ingresos, el comportamiento de los clientes, el desempeño logístico y los factores de churn**, transformando datos transaccionales en **insights accionables de negocio**.

Más allá de métricas descriptivas, el análisis busca responder una pregunta estratégica central:

> **¿Por qué un marketplace con alta satisfacción del cliente presenta niveles de churn tan elevados?**

---

## 🎯 Objetivos de Negocio
- Identificar **categorías líderes** por volumen, revenue y ticket promedio  
- Analizar el **comportamiento de compra por día de la semana**  
- Medir el impacto de los **retrasos en la entrega sobre la satisfacción**  
- Detectar **sellers de alto riesgo** más allá de la logística  
- Segmentar clientes mediante **análisis RFM**  
- Evaluar **churn, LTV y sostenibilidad del modelo**  
- Analizar el **costo del flete como barrera estructural**  
- Identificar **oportunidades de expansión geográfica**

---

## 📊 Fuentes de Datos
- Órdenes y productos  
- Clientes y sellers  
- Pagos  
- Reviews  
- Geolocalización y costos de flete  

Dataset público: **Olist Brazilian E-Commerce Dataset**.

---

## 🔑 Insights Clave 

### 1️⃣ Concentración de Revenue por Categoría
Las categorías con mayor volumen de órdenes y revenue son:
- **Health & Beauty**
- **Bed, Bath & Table**
- **Sports & Leisure**
- **Computers & Accessories**

📌 **Insight:**  
El revenue se explica por dos estrategias distintas:
- Categorías de **alta frecuencia**  
- Categorías de **alto valor por ticket**

---

### 2️⃣ Categorías Premium: Valor sin Escala
Top 5 categorías por **Ticket Promedio**:
- Computers (R$ 1.147)
- Electrodomésticos
- Agroindustria
- Instrumentos musicales

📌 **Implicancia:**  
Son categorías que **aportan margen**, pero no volumen. Su rentabilidad depende fuertemente de la eficiencia logística.

---

### 3️⃣ El “Efecto Lunes” y la “Paradoja del Sábado”
- **Lunes:** mayor cantidad de órdenes (15.701)  
- **Sábado:** menos órdenes (10.555), pero **ticket promedio más alto (R$ 144)**

🧠 **Insight de comportamiento:**  
El fin de semana se toman decisiones más racionales y de mayor valor; entre semana predominan compras rutinarias.

---

### 4️⃣ Retrasos y Experiencia del Cliente: el Punto de Quiebre
Existe un umbral claro de tolerancia al retraso:

| Retraso | Comportamiento |
|------|---------------|
| ≤ 3 días | 65% de reviews positivas |
| 4–7 días | Las reviews negativas se triplican |
| > 15 días | 78.9% de reviews negativas |

📌 **Conclusión:**  
A partir del **día 4**, la experiencia entra en zona crítica y el riesgo de churn se dispara.

---

### 5️⃣ Sellers de Alto Riesgo: No es un Problema Logístico
Los sellers con mayor porcentaje de reviews negativas:
- Entregan **antes de lo prometido**
- Aun así tienen **50–60% de reviews negativas**

🎯 **Insight Pro:**  
El problema es **calidad del producto o expectativas**, no logística. La velocidad no compensa una mala experiencia.

---

Segmentación por clientes: 
El 65.9% de los clientes son "Prometedores". Estos clientes están a una mala experiencia (o un flete caro) de desaparecer. No tienen historial de lealtad; son "prometedores" solo porque compraron hace poco, pero su LTV ($164) es casi idéntico al de los clientes que ya diste por perdidos ("Lost", $165).
En el segmento "Lost" (clientes que no han vuelto en más de un año), el 56.9% de las órdenes tuvieron un flete Alto o Muy Alto (más del 20% del valor del producto).
Casi 6 de cada 10 clientes que perdiste pagaron un "impuesto" logístico carísimo. Es muy probable que su experiencia de compra haya terminado con un sentimiento de "me salió más caro el collar que el perro", anulando cualquier posibilidad de recompra.
Tanto en Lost como en Others, el porcentaje de clientes con Flete Bajo (<10%) es el más pequeño (aprox. 15.4% - 15.6%).
 Esto sugiere que los clientes con fletes bajos son los que NO están en estas listas de "perdidos" en la misma proporción. O dicho de otra forma: si el flete es bajo, el cliente tiene muchas más probabilidades de migrar hacia un segmento de mayor lealtad en lugar de quedarse estancado en "Others" o morir en "Lost".


Categorías de "Repuesto" (Home Appliances y Drinks): Con un 19% y 15.6% de recompra, vemos que el cliente vuelve cuando el producto es de consumo o necesidad funcional inmediata.El fenómeno "Fashion": Las categorías de bolsos y accesorios están en el Top 3. Esto sugiere que hay un componente emocional o de catálogo que invita a explorar más de una vez.El fracaso de la tecnología: Computadoras y electrónica tienen las tasas más bajas ($2.27\%$). Nadie compra una PC dos veces en un año. Aquí el flete duele más porque el producto es caro y la expectativa de logística es altísima.


### 8️⃣ El Flete como Barrera de Crecimiento
**Freight-to-Price Ratio promedio: 0.32**

- Norte y Nordeste: **55–60%**
- São Paulo: **0.26**
- Mediana: **0.23**

🚧 **Insight:**  
El flete no es un costo adicional, es una **barrera a la recompra**, especialmente en regiones alejadas.

---

### 9️⃣ São Paulo: El Pulmón del Sistema
- Genera **R$ 5.7M**, más que todas las demás regiones combinadas  
- Menor costo promedio de flete (R$ 15.1)

📌 **Conclusión:**  
Olist es un negocio de **proximidad logística**, no un mercado homogéneo a nivel nacional.

---

### 🔟 Regiones con Mejor Potencial de Expansión
**Centro-Oeste y Sur (DF, PR):**
- Ticket promedio saludable (R$ 126–138)
- Flete estable (~0.34)

🎯 **Estrategia recomendada:**  
Zonas ideales para **membresías tipo Prime** o **flete fijo**.

---

## 📈 KPIs Principales

| KPI | Valor | Interpretación |
|---|---|---|
| SLA Compliance | 92.09% | Alta estabilidad operativa |
| Ticket Promedio | R$ 159.83 | Ancla económica |
| NPS | 62.06 | Alta satisfacción |
| Churn | 59.8% | Retención deficiente |
| Freight-to-Price | 0.32 | Fricción estructural |

---

## 🧠 Conclusión Final de Negocio
Olist es **muy eficiente captando clientes y cumpliendo entregas**, pero **ineficiente reteniéndolos**.

Los clientes están satisfechos, el sistema funciona, pero:

> **El costo de volver a comprar (flete) supera el valor percibido de la recompra.**

Esto convierte al marketplace en un modelo **transaccional, frágil y dependiente del CAC**.

---

## 🚀 Recomendaciones Estratégicas
- Incentivos de flete para la **segunda compra**
- Estrategias logísticas regionalizadas
- Control de calidad para sellers de alto riesgo
- Redefinir “lealtad” (2 compras = cliente elite)
- Priorizar retención antes de escalar adquisición

---

## 🛠️ Herramientas Utilizadas
- R / tidyverse  
- SQL  
- Visualización con ggplot2  
- Segmentación RFM  
- Modelado de KPIs de negocio  

---



