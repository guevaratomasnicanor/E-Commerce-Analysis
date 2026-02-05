# E-Commerce-Analysis
Tus datos revelan que el cliente de Olist es "tolerante" hasta el tercer día de retraso. A partir del cuarto día, la experiencia de usuario entra en zona de desastre:

Zona Segura (≤ 3 días tarde): La satisfacción (4-5⭐) se mantiene en un aceptable 65%.

Zona de Riesgo (4-7 días tarde): El porcentaje de reviews negativas (≤ 2⭐) se triplica al 62.2%.

Zona Crítica (> 15 días tarde): El 78.9% de los clientes califica negativamente. Aquí el riesgo de churn es casi total.

Es muy interesante notar que el top 10 de vendedores con mayor riesgo tienen un avg_delay negativo (llegan antes de tiempo), pero un pct_negative_reviews altísimo (cerca del 50-60%).

Insight Pro: Esto sugiere que el problema de estos vendedores no es la logística, sino la calidad del producto o la expectativa. Están entregando rápido, pero lo que entregan decepciona profundamente al cliente.

2. Sellers de "Alto Riesgo"
Es muy interesante notar que el top 10 de vendedores con mayor riesgo tienen un avg_delay negativo (llegan antes de tiempo), pero un pct_negative_reviews altísimo (cerca del 50-60%).

Insight Pro: Esto sugiere que el problema de estos vendedores no es la logística, sino la calidad del producto o la expectativa. Están entregando rápido, pero lo que entregan decepciona profundamente al cliente.


El 85.6% de tus clientes están en el segmento "Need Attention" con una frecuencia promedio de 1.

Esto significa que la gran mayoría de los usuarios entra, compra una vez y no vuelve.

Riesgo: Si el costo de adquirir un cliente (CAC) es alto, el negocio es frágil porque no hay recompra orgánica que amortice ese gasto.

2. Los "Loyal Customers" son una anomalía
Solo encontraste 3 clientes en el segmento Loyal.

Esto sugiere que los cortes de tus quintiles (breaks = 5) podrían estar demasiado apretados porque casi no hay variación en la frecuencia. En Olist, alguien que compra 2 veces ya es un cliente de élite.

3. El Segmento "At Risk" (14.4%)
Tienes 13,843 clientes que compraron hace mucho tiempo (recencia promedio de 502 días) y nunca volvieron. este grupo representa capital muerto: usuarios que ya conocen la plataforma pero que el servicio o el precio no logró retener.


La tasa de churn global del 59.8% confirma que el modelo actual es puramente transaccional. En términos de riesgo, esto significa que el flujo de caja futuro es altamente incierto porque depende casi exclusivamente de captar clientes nuevos constantemente.

🔍 Hallazgos Críticos por Segmento
1. La fragilidad del "Loyal Customer"
Dato: Aunque tienen un LTV impresionante ($6,760 vs $159 del promedio), solo son 3 personas y una ya entró en churn (33.3%).

Insight de Riesgo: No se puede construir un modelo de estabilidad basado en anomalías. El verdadero riesgo es que el 85% del revenue depende del segmento "Need Attention", que tiene un churn del 53%.

2. El Segmento "At Risk" como Costo de Oportunidad
Tienes 13,843 clientes con un 100% de churn. Estos usuarios ya gastaron dinero una vez ($163 en promedio), pero Olist no logró retenerlos.

Impacto Financiero: Si se lograra reactivar solo al 10% de este grupo, recuperarías más de $225,000 en ventas sin costo de adquisición inicial.

3. El Valor de Vida (LTV) Estancado
La diferencia entre el LTV de un cliente en riesgo ($163) y uno activo ($159) es mínima. Esto sugiere que los clientes no crecen dentro de la plataforma; se quedan en su ticket inicial y luego se van.



1. La Barrera del 50%: El flete como inhibidor de compra
El indicador Freight-to-Price Ratio muestra una desigualdad geográfica masiva en Brasil.

El Muro del Norte: En estados como Rondônia (RO), Roraima (RR) y Maranhão (MA), el costo del flete representa entre el 55% y 60% del valor del producto.

Efecto en el Ticket: Para que el flete sea "pagable" en estas regiones, el ticket promedio tiende a ser más alto ($167 en RO vs. $109 en SP).

Insight de Datos: Olist es un negocio de proximidad. En el Norte y Noreste, el flete no es un "añadido", es una barrera que probablemente está causando un abandono de carrito masivo que no vemos en estos datos de órdenes completadas.

2. São Paulo: El pulmón del sistema
La dominancia de SP no es solo por población, es por eficiencia logística.

Con un ratio de flete de 0.26 (el más bajo), SP genera $5.7 millones en ingresos, más que todas las demás regiones combinadas.

Dato Clave: SP tiene el flete promedio más bajo ($15.1), lo que permite la venta de productos de bajo ticket que en otros estados serían inviables.

3. El "Sweet Spot" del Centro-Oeste y Sur
Estados como Distrito Federal (DF) y Paraná (PR) presentan el mejor equilibrio para la expansión:

Tienen tickets promedio saludables ($126 - $138).

Mantienen ratios de flete competitivos (~0.34).

Estrategia: Estas regiones son los mejores candidatos para programas de "Flete Fijo" o membresías tipo Prime, ya que el costo logístico es predecible y no erosiona el margen del cliente.


🗺️ Hotspots y Categorías Regionales
Especialización del Norte/Noreste: Las categorías de Health & Beauty y Watches/Gifts dominan los ingresos en las regiones alejadas. Al ser productos de poco peso y alto valor, son los únicos que logran absorber el costo del flete sin espantar al comprador.

Concentración Urbana: Solo São Paulo y Río de Janeiro concentran casi el 45% del revenue total de los hotspots. Fuera de las capitales, el e-commerce en Brasil todavía tiene un techo logístico muy marcado.


SLA Compliance (92.09%): Es una métrica de estabilidad alta. Nueve de cada diez pedidos cumplen con la promesa de entrega. Sin embargo, en un volumen de 110k órdenes, ese ~8% de fallas representa a miles de usuarios que entran directamente en la "zona de riesgo" de insatisfacción que vimos antes.

Average Order Value (R$ 159.83): Este es tu ancla económica. Cualquier costo operativo (como el flete o el marketing) debe medirse contra estos 160 reales para entender si la transacción es rentable.

NPS (62.06 puntos): Un puntaje de 62 es sólido. Indica que la mayoría de los usuarios son "Promotores". Esto confirma que el problema de Olist no es el producto o el servicio base, sino la falta de incentivos para la recurrencia (como vimos en el Churn del 60%).

Freight-to-Price Ratio (0.32): La diferencia entre el promedio (0.32) y la mediana (0.23) es un indicador de distorsión. El flete promedio es más alto porque las entregas a zonas remotas tienen costos tan extremos que "mueven" la media, a pesar de que la mayoría de las órdenes tienen un costo de envío más bajo.


📉 Análisis de Rendimiento (KPIs)
SLA Compliance (92.09%): Es una métrica de estabilidad alta. Nueve de cada diez pedidos cumplen con la promesa de entrega. Sin embargo, en un volumen de 110k órdenes, ese ~8% de fallas representa a miles de usuarios que entran directamente en la "zona de riesgo" de insatisfacción que vimos antes.

Average Order Value (R$ 159.83): Este es tu ancla económica. Cualquier costo operativo (como el flete o el marketing) debe medirse contra estos 160 reales para entender si la transacción es rentable.

NPS (62.06 puntos): Un puntaje de 62 es sólido. Indica que la mayoría de los usuarios son "Promotores". Esto confirma que el problema de Olist no es el producto o el servicio base, sino la falta de incentivos para la recurrencia (como vimos en el Churn del 60%).

Freight-to-Price Ratio (0.32): La diferencia entre el promedio (0.32) y la mediana (0.23) es un indicador de distorsión. El flete promedio es más alto porque las entregas a zonas remotas tienen costos tan extremos que "mueven" la media, a pesar de que la mayoría de las órdenes tienen un costo de envío más bajo.

💡 Insight de Datos Consolidado
Si conectamos los puntos:

Tienes un AOV de R$ 160.

Un flete que consume el 32% de ese valor en promedio.

Un NPS alto (la gente está contenta).

Pero un Churn masivo.

Conclusión técnica: El sistema es excelente captando y cumpliendo, pero es ineficiente reteniendo. El alto costo del flete en relación al ticket promedio actúa como un impuesto a la recurrencia. El cliente queda satisfecho con su compra, pero el costo de "volver a pedir" (flete) comparado con el valor del producto parece no compensar.
