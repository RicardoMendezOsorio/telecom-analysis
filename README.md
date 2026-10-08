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

## 🧠 Hallazgos del análisis

1. Mediante un análisis IQR se detectaron outliers para las columnas cant_mensajes, cant_llamadas y cant_minutos_llamadas (46, 30, 109 datos respectivamente), sin embargo no se decidio tomar alguna acción con estos datos ya que la cantidad de mensajes, llamadas y minutos varia con el uso de cada usuario y los datos son plausibles.
2. En el análisis se identificaron a los usuarios en segnmentos de edad obteniendo que los más predominantes son los adultos (2,018 usuarios equivalentes al 50.45% que tienen edades entre los 30 y 60 años), despues vienen los adultos mayores(1,222 usuarios equivalentes al 30.55% con edades superiores a los 60 años) y finalmente los jovenes(760 usuarios equivalentes al 19% que son menores de 30 años)
3. Aunado a esto se hizo un análisis por el plan contratado (básico o premium) teniendo que del total de usuarios el 64.87% tiene contratado el plan básico, mientras el 35.13% cuenta con el plan premium. Y de este porcentaje con respecto a la edad de los usuarios se tiene que para el plan básico corresponde a los adultos el 51.05%, para adultos mayores el 30.22% y para jovenes el 18.73%. Mientra que para el plan premium corresponde a los adultos el 49.33%, para adultos mayores el 31.17% y para jovenes el 19.50%. Observando un comportamiento similar conforme al plan y edad de los usuarios.
4. En el análisis se identificaron a los usuarios en segnmentos de uso obteniendo que los más predominantes son los uso medio (2,917 usuarios equivalente al 73.57%), despues vienen los bajo uso(766 usuarios equivalente al 19.45%), los alto uso(276 usuarios equivalente al 6.95%) y se detecta un caso particular de un usuario el cual no hizo uso del servicio ni para mensajes y llamadas, por lo que se considera como Uso nulo (1 usuario equivalente al 0.03%)
5. Aunado a esto se hizo un análisis por el plan contratado (básico o premium) teniendo que del total de usuarios el 64.87% tiene contratado el plan básico, mientras el 35.13% cuenta con el plan premium Y de este porcentaje con respecto al uso de los usuarios se tiene que para el plan básico corresponde a uso medio el 73.10%, para bajo uso el 19.73%, para alto uso el 7.13% y para Uso nulo el 0.04%. Mientra que para el plan premium corresponde a los uso medio el 74.45%, para bajo uso el 18.93% y para alto uso el 6.62%. Observando un comportamiento similar conforme al plan y uso de los usuarios.

## 🧠 Recomendaciones

1. Se puede análisar que otras variables influyen en la elección de plan en el dataset como puede ser la ciudad o las fechas de contratación
2. Establecer una campaña de beneficios para los usuarios de alto y medio uso para que decidan cambiar al plan premium haciendo notar los beneficios que obtendrian
3. Enfocar atraer a usuarios más jovenes ofreciendo un plan que se adapte a las necesidades de ese sector de mercado (universitarios, creadores digitales, redes sociales, más GB, etc)

## 📂 Contenido del repositorio

- `nS7 Version-Estudiante-Project-ConnectaTel.ipynb`
  → Notebook principal con limpieza, EDA, distribuciones, outliers y conclusiones.

## ▶ Cómo abrir el notebook 

Haz clic en el siguiente botón:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `S7 Version-Estudiante-Project-ConnectaTel.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)


