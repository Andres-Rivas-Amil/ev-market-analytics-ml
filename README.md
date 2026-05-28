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


  
