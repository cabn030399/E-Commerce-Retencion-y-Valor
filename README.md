# E-Commerce Customer Retention & Churn Predictive Analysis
### Proyecto de Portafolio - Analista de Datos Certificado (TripleTen Latam)

## 📌 1. Definición del Problema de Negocio
El equipo de marketing y retención de un e-commerce global identificó una desaceleración en el crecimiento sostenido debido a una alta tasa de abandono tras la primera compra. El costo de adquisición de clientes (CAC) se ha incrementado, por lo que el objetivo principal es identificar qué patrones de comportamiento distinguen a los clientes recurrentes de los que abandonan, definir un umbral científico de inactividad (Churn) y proponer recomendaciones accionables.

## 🛠️ 2. Tecnologías y Herramientas Utilizadas
* **Python 3.11 (Entorno Virtual Aislado):** `Pandas` para manipulación de datos, `NumPy` para lógica algorítmica, `Matplotlib` y `Seaborn` para análisis exploratorio (EDA).
* **VS Code:** Entorno de desarrollo para cuadernos de Jupyter.
* **Tableau Public:** Construcción de un Dashboard interactivo para la toma de decisiones ejecutivas.

## 📐 3. Metodología Analítica Avanzada
* **Pipeline de Limpieza:** Remoción de registros nulos en `CustomerID`, aislamiento de transacciones de devolución (códigos 'C' en `InvoiceNo`) y corrección de anomalías de precio.
* **Segmentación RFM Estadistica:** Creación de scores del 1 al 5 basados en cuantiles de la población para Recencia, Frecuencia y Valor Monetario, clasificando la base en 6 perfiles comerciales (*Campeones VIP, Clientes Leales, En Riesgo Alto*, etc.).
* **Definición Científica de Churn:** Análisis del *Tiempo Entre Visitas* de compradores recurrentes. Utilizando el **Percentil 80** de la distribución empírica, se determinó que el ciclo natural de recompra del negocio es de **52 días** y el umbral límite de tolerancia es de **112 días**.

## 📊 4. Insights Clave (Resultados del Modelo)
* **Ley de Pareto:** El segmento **Campeones (VIP)** representa únicamente el **14.96%** de la base total de clientes, pero concentra el **59.16% de los ingresos totales** de la tienda (£5,272,208).
* **Calibración de Riesgo:** El grupo **En Riesgo Alto** concentra a 567 clientes que solían ser recurrentes pero promedian **158 días de inactividad**, superando el umbral de Churn.
* **Tasa de Abandono:** La **Tasa de Churn Global** se sitúa en **29.46%**, un rango saludable para la industria minorista, pero controlable mediante alertas tempranas.

## 🎯 5. Recomendaciones Estratégicas para Negocio
1. **Blindaje VIP:** No otorgar cupones masivos de descuento al segmento *Campeones (VIP)* ya que su intención de compra es orgánica. Se sugieren programas de lealtad por puntos o accesos exclusivos a lanzamientos.
2. **Campañas de Rescate (En Riesgo Alto):** Configurar triggers automatizados de marketing (Email / WhatsApp) exactamente al **día 50 de inactividad** (previo a la ventana natural de recompra de 52 días) ofreciendo un incentivo personalizado para reactivar al cliente antes de que cruce el umbral de los 112 días y se convierta en Churn definitivo.
3. **Optimización de Presupuesto:** Cesar de inmediato las campañas agresivas de pauta publicitaria digital dirigidas a los usuarios *Perdidos e Inactivos*, dado que su costo de reactivación supera el valor futuro estimado (LTV).

---
▶️ **[Haz clic aquí para interactuar con el Dashboard en Tableau Public][](https://public.tableau.com/views/Retail_17934189080760/Dashboard1?:language=es-ES&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link))**
