# ventas-autos

# Análisis de Ventas de Autos en Databricks CE

**Asignatura:** Big Data  
**Año:** 2025  
**Estudiantes:** Oscar Javier García, Rober Andrés Gaviria  
**Profesor:** Andrés Felipe Callejas  

---

## **1. Descripción del Proyecto**
Este proyecto tiene como objetivo analizar un conjunto de datos de ventas de automóviles, utilizando **Databricks CE** y **Apache Spark**. Se aplica tanto **SQL** como la **API de DataFrames de Spark** para:

- Ingesta de datos desde Kaggle.  
- Limpieza y transformación de datos.  
- Creación de tablas Delta.  
- Validaciones y análisis exploratorio de datos.  
- Comparativa de ventajas y desventajas entre SQL y Spark.  
- Visualización de información relevante como ventas por fabricante y distribución de precios.

---

## **2. Objetivos**
1. Diseñar un esquema adecuado para el conjunto de datos.  
2. Configurar el entorno en Databricks CE y cargar los datos.  
3. Realizar limpieza y transformación de datos, incluyendo validación de nulos y duplicados.  
4. Crear tablas Delta para un manejo eficiente de los datos.  
5. Comparar la eficiencia y flexibilidad entre consultas SQL y DataFrames de Spark.  
6. Generar visualizaciones para análisis exploratorio.  

---

## **3. Estructura del Proyecto**
Proyecto_Databricks/
│
├─ notebooks/
│ ├─ 01_ingesta_schema.ipynb # Notebook de ingestión y definición de esquema
│ ├─ 02_limpieza_transformacion.ipynb# Limpieza y transformaciones
│ ├─ 03_validacion_sql_spark.ipynb # Validaciones y comparativa SQL vs Spark
│ └─ 04_analisis_visual.ipynb # Visualización de resultados
│
├─ data/
│ └─ ventas_autos.csv # Archivo CSV de datos de autos
│
├─ scripts/
│ └─ funciones_utiles.py # Funciones auxiliares (opcional)
│
├─ results/
│ └─ graficos/ # Carpeta para guardar gráficos generados
│
└─ README.md # Este archivo

yaml
Copiar código

---

## **4. Tecnologías Utilizadas**
- **Databricks CE**  
- **Apache Spark** (DataFrame API)  
- **SQL**  
- **Python**  
- **Pandas, Matplotlib y Seaborn** para visualizaciones  

---

## **5. Instrucciones de Uso**
1. Clonar este repositorio:
```bash
git clone https://github.com/usuario/ventas_autos_databricks.git
Abrir los notebooks en Databricks CE.

Subir el archivo ventas_autos.csv a /FileStore/tables si no está incluido.

Ejecutar las celdas de cada notebook en orden:

01_ingesta_schema.ipynb

02_limpieza_transformacion.ipynb

03_validacion_sql_spark.ipynb

04_analisis_visual.ipynb

Revisar gráficos, tablas y resultados generados en los notebooks.

6. Resultados Esperados
Tabla Delta creada: autos.ventas_autos.

Validaciones de datos completadas (nulos, duplicados, rangos correctos).

Visualizaciones:

Ventas por fabricante.

Distribución de precios y eficiencia de combustible.

Comparativa de consultas SQL vs Spark.

7. Créditos
Estudiantes: Oscar Javier García, Rober Andrés Gaviria

Profesor: Andrés Felipe Callejas

Fuente de datos: Kaggle – Ventas de autos

8. Buenas Prácticas
Mantener notebooks numerados para facilitar la ejecución secuencial.

Evitar subir archivos grandes al repositorio.

Hacer commits frecuentes con mensajes descriptivos.

Documentar cada notebook y celda con Markdown.
