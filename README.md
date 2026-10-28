# 🛍️ Sprint 7 · Proyecto de ventas multicanal LATAM
## 📊 Análisis exploratorio de datos con Python para comprender los ingresos, la rentabilidad y el comportamiento de ventas de una tienda multicanal en Latinoamérica.
## 🎯 Objetivo del proyecto
Analizar un conjunto de datos de ventas multicanal para identificar patrones por país, canal y categoría; revisar la calidad de los datos; calcular indicadores clave de negocio (KPIs); detectar posibles valores atípicos y segmentar las ventas por nivel de ingreso.
El proyecto es una práctica guiada de nivel introductorio-intermedio para aprender un flujo de trabajo de análisis de datos y comunicar hallazgos con evidencia.
🗂️ Dataset utilizado
El notebook utiliza el archivo CSV sprint07_proyecto_ventas_multicanal_latam.csv, que se carga desde esta URL pública:

## 🔗 Abrir dataset CSV

El dataset contiene información de ventas, ubicación, canal, categoría, cliente, ingresos, costos, margen y experiencia de entrega. Algunas columnas importantes son:
Campo	Descripción
venta_id	Identificador de la venta
fecha	Fecha de la venta
pais, region, ciudad	Ubicación de la operación
canal	Web, App, Tienda física o WhatsApp
categoria	Categoría del producto
metodo_pago	Medio de pago
tipo_cliente	Cliente nuevo o recurrente
unidades, precio_unitario, descuento_pct	Datos de la compra
ingreso, costo, margen	Métricas económicas
edad_cliente, satisfaccion, dias_entrega	Variables del cliente y su experiencia
devolucion	Indica si la venta fue devuelta


⚠️ Nota: si la URL deja de estar disponible, descarga el CSV y actualiza la variable archivo con la ruta local o de Google Drive.

## 🔎 Etapas del análisis
1. 🧭 Exploración inicial: visualizar registros, dimensiones, nombres de columnas y tipos de datos.
2. 🧪 Calidad de datos: contar valores nulos y calcular su porcentaje por columna.
3. 🧹 Limpieza: crear una copia de trabajo (df_limpio), convertir fechas, normalizar textos y completar valores faltantes según las reglas planteadas.
4. ⚙️ Automatización: practicar ciclos y funciones para revisar columnas y reducir tareas repetitivas.
5. 📌 KPIs de negocio: calcular ingreso total, margen total y porcentual, ticket promedio, tasa de devolución y satisfacción promedio.
6. 📈 Visualización: crear gráficos de ingresos por país, categoría y mes, además de histogramas.
7. 🎨 Comparación de grupos: utilizar Seaborn y hue para comparar canales, categorías y tipos de cliente.
8. 🚩 Detección de valores atípicos: aplicar el rango intercuartílico (IQR) para localizar ventas que conviene revisar.
9. 🧩 Segmentación: clasificar las ventas por nivel de ingreso (bajo, medio y alto).
10. 💡 Conclusión de negocio: preparar una tabla con resultados por país, canal y categoría, y proponer acciones respaldadas por datos.
## 🧰 Herramientas utilizadas
- 🐍 Python — lenguaje de programación.
- 🐼 Pandas — carga, limpieza, agrupación y análisis tabular.
- 🔢 NumPy — operaciones numéricas, si se requieren.
- 📊 Matplotlib — gráficos.
- 🎨 Seaborn — visualizaciones estadísticas.
- ☁️ Google Colab / Jupyter Notebook — entorno de ejecución.
## 🚀 Cómo ejecutar el notebook en Google Colab
1. Descarga o guarda el notebook Copia_de_Sprint07_Webinar11_students_version.ipynb.
2. 🌐 Abre Google Colab.
3. Selecciona Archivo → Subir notebook y carga el archivo .ipynb.
4. Verifica que el entorno tenga conexión a internet para leer el CSV desde la URL incluida en el notebook.
5. ▶️ Ejecuta las celdas en orden, desde el inicio hasta el cierre, con Entorno de ejecución → Ejecutar todas o Shift + Enter para una celda a la vez.
6. Si necesitas instalar las librerías, ejecuta:
   !pip install pandas matplotlib seaborn
7. Revisa las tablas, gráficos y conclusiones. Si cambias alguna regla de limpieza, vuelve a ejecutar las celdas posteriores para actualizar los resultados.
## 🔁 Guía breve de reproducción
1. Usa el notebook y el CSV indicados en este README.
2. Ejecuta las celdas en orden en una sesión nueva de Colab.
3. Confirma que la carga del CSV se complete correctamente.
4. Revisa dimensiones, tipos de datos y valores nulos del dataset original.
5. Ejecuta las transformaciones y comprueba los resultados de df_limpio.
6. Verifica los KPIs, las visualizaciones, los posibles outliers y la columna segmento_ingreso.
7. Consulta la tabla final ordenada por ingreso y redacta una conclusión con hallazgo, evidencia e implicación para el negocio.
## 📝 Importante: conserva el dataset original y trabaja sobre df_limpio. Los resultados dependen de la versión del CSV y de las decisiones de limpieza y segmentación aplicadas.

⚠️ Consideraciones y limitaciones
- Los valores atípicos no son necesariamente errores; deben interpretarse antes de excluirlos.
- La imputación de valores faltantes puede afectar las métricas, por lo que conviene documentar las decisiones.
- Los umbrales de segmentación de ingresos son reglas de práctica del notebook y pueden ajustarse según el contexto del negocio.
- El análisis describe patrones del dataset; por sí solo no demuestra causalidad.
## 👤 Autoría
- Autor/a: ALEJANDRRO VALENCIA LOPEZ
- Proyecto: Sprint 7 · Proyecto de ventas multicanal LATAM
