# ev-market-analytics-ml
Análisis integral del mercado global de vehículos eléctricos 2026. Incluye ingeniería de datos, modelos de Machine Learning (Random Forest) para predicción de precios/ventas en Python y dashboards interactivos en Power BI

# ⚡ Dashboard de Análisis del Mercado de Vehículos Eléctricos (2026)

¡Bienvenido/a a mi proyecto de Business Intelligence sobre el mercado global de vehículos eléctricos! Este informe interactivo de Power BI ha sido diseñado bajo un enfoque "Eco-Tech", priorizando una estructura limpia, consistente y altamente corporativa para la toma de decisiones estratégicas.

## 🚀 Características Principales
* **Diseño UX Interactivo:** Portada con botones de navegación integrados y botones de "Home" en todas las páginas para una experiencia de usuario fluida.
* **Panel de Control Centralizado:** Pestaña dedicada exclusivamente a la gestión de filtros globales sincronizados.
* **Análisis de Negocio (Dashboard Ventas):** Estudio de ingresos globales, volumen de unidades vendidas, distribución por segmentos y evolución temporal del mercado.
* **Análisis Técnico y Satisfacción (Dashboard Producto):** Matriz de competitividad cruzando Autonomía vs. Velocidad de Carga, además de KPIs específicos de rendimiento (Tracción, Potencia, Aceleración) y valoraciones de los usuarios.
* **Ficha Técnica (Dataset):** Una tabla interactiva de consulta avanzada optimizada para auditoría de datos y exportación a Excel.

## 📊 Vista Previa del Reporte
*Aquí puedes insertar las capturas de pantalla de tu carpeta `/screenshots` para que luzca increíble:*

### Portada
![Portada](./screenshots/image_c9346b.png)

### Dashboard de Ventas
![Ventas](./screenshots/image_c934a9.png)

### Dashboard de Producto y Satisfacción
![Producto](./screenshots/image_c93507.png)

## 🛠️ Tecnologías Utilizadas
* **Power BI Desktop** (Modelado de datos, DAX, Diseño de Interfaz y Navegación)
* **Python / Pandas** (Análisis exploratorio previo del dataset)
* **Markdown** (Documentación del repositorio)

## 🧠 Fase 1: Ingeniería de Datos y Machine Learning (Python & Jupyter)
Antes del diseño visual en Power BI, se procesó el dataset original de 2,000 registros mediante un pipeline completo en un entorno Jupyter Notebook (`Estudio coches electricos.ipynb`).

### 🔍 Análisis Exploratorio (EDA) y ETL
* **Calidad de Datos:** Auditoría automatizada de tipos de datos, verificación de valores nulos y análisis de duplicados.
* **Transformaciones:** Limpieza estructural de variables numéricas y tratamiento de categorías categóricas mediante encoding para los algoritmos de predicción.

### 🤖 Modelado Predictivo e Insights de Negocio
Se entrenaron modelos basados en **Bosques Aleatorios (Random Forest Regressor)** para analizar el comportamiento del mercado con dos enfoques:

1. **Predicción de Volumen de Ventas (`annual_sales_units`):**
   * **Insight Clave:** La **Marca** domina el modelo con una importancia de feature de **0.813**. El branding es el motor principal que tracciona las unidades vendidas en el mercado global.
2. **Predicción de Estrategia de Precios (`price_usd`):**
   * **Insight Clave:** La marca pasa a ser casi irrelevante (peso de 0.049). El precio está anclado a factores técnicos y de mercado: la **Potencia (0.464)** y el **Segmento (0.338)** explican el 80% de la variabilidad del coste.
   * **Análisis de Residuos:** Distribución simétrica y centrada en $0 (sesgo mínimo), confirmando la robustez del modelo predictivo no lineal frente a modelos lineales tradicionales.

## 🎯 Enfoque Metodológico y Objetivos de Negocio

Este proyecto no se limitó a explorar datos al azar; se diseñó bajo una metodología estructurada orientada a resolver necesidades del sector automotriz. Antes de iniciar la fase técnica, se desarrolló un **Plan Analítico** con 8 casos de uso estratégicos.

Puedes consultar el documento de planificación original aquí:
* [📋 Plan de Análisis y Casos de Uso (PDF)](./docs/Plan_Analitico_Mercado_EV.pdf)

### 📈 Casos de Uso Clave Abordados:
De los objetivos planteados en la estrategia, el proyecto resuelve con éxito los núcleos analíticos más complejos:
* **Predicción de Precios y Ventas (Casos 1 y 7):** Implementación del modelo *Random Forest* en Python, descubriendo el fuerte impacto de la marca en el volumen de ventas (0.813) frente al peso del rendimiento en el precio final (0.464).
* **Análisis de Valor y Segmentación (Casos 2, 3 y 8):** Mapeo en Power BI de la relación Autonomía vs. Precio, contrastando el segmento económico (<$35k) frente al de lujo (>$100k) y evaluando la eficiencia de millas por dólar.
* **Evolución Tecnológica y Ventas 2020-2026 (Casos 4 y 5):** Dashboards interactivos que muestran la trayectoria de la capacidad de las baterías, velocidades de carga y cuotas de mercado a lo largo de los últimos 6 años.
  
