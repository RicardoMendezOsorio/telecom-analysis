# Telecom-analysis – Sprint 7

Este repositorio contiene el análisis realizado durante el Sprint 7 del caso ConnectaTel.

## 🧠 Objetivo del análisis

- Integrar y limpiar bases de datos provenientes de tres fuentes distintas.
- Aplicar técnicas de validación, estandarización de tipos de datos y detección de valores inconsistentes.
- Construir un perfil estadístico del uso (llamadas y mensajes) por cliente y por segmentos demográficos.
- Detectar outliers y comportamientos atípicos mediante métodos estadísticos y visuales.
- Crear segmentaciones de clientes basadas en edad, país y comportamiento de uso.
- Visualizar diferencias entre segmentos y extraer insights comerciales relevantes.
- Documentar todo el proceso en un Jupyter Notebook, junto con un README reproducible para subirlo a GitHub.

-Los datasets utilizados son: 
plans.csv: Catálogo de planes con sus precios y beneficios. 
users_latam.csv: Información de cada usuario (datos personales, plan, fecha de registro, churn). 
usage.csv: Actividad generada por los usuarios: llamadas, mensajes, duración, longitud. 

## 📂 Etapas del análisis

1. Cargar y explorar
2. Identificar problemas de calidad
3. Limpieza básica
4. Summary statistics
5. Visualización y outliers
6. Segmentación
7. Insight ejecutivo
8. Publicación 

## 📂 Contenido del repositorio

- `notebooks/S7 Version-Estudiante-Project-ConnectaTel.ipynb`
  → Notebook principal con limpieza, EDA, distribuciones, outliers y conclusiones.

## ▶ Cómo abrir el notebook 

Haz clic en el siguiente botón:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/S7 Version-Estudiante-Project-ConnectaTel.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)


