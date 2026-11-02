# ConnectaTel Analysis

Telecom customer analysis for ConnectaTel in Latin America, using data up to 2024.

## Question
Evaluate customer behaviour to build a statistical customer profile, detect atypical behaviour, create customer segments, identify consumption patterns, design retention strategies, and suggest plan improvements.

## Datasets
- `plans.csv` — 2 plans, 8 columns
- `users_latam.csv` — 4,000 users, 8 columns (age, city, registration date, plan, churn date)
- `usage.csv` — 40,000 records, 6 columns (calls and messages, date, duration/length)

Plans shown: Básico — 100 messages, 5 GB, 100 minutes, $12/month. Premium — 500 messages, 20 GB, 600 minutes, $25/month.

## Tools
Python, Pandas, NumPy, Seaborn, Matplotlib, Jupyter Notebook.

## What I did
Load and explore the three datasets, clean the data, build a `user_profile` table with message counts, call counts and call minutes, segment customers by use and by age, and visualise the results.

Segments used:
- Use: Low use (calls < 5 and messages < 5), Medium use (calls < 10 and messages < 10), High use (the rest)
- Age: Young (< 30), Adult (30–59), Older adult (≥ 60)

## Key findings
- Data quality issues found: age = -999, city = "?", future dates, and nulls in duration and length (5–20%).
- Young and adult high-use customers are more active in messages and calls.
- Most valuable customers identified qualitatively: high-use young and adult customers, with higher loyalty potential.
- Outliers: some users with extreme use, who may be strategic customers or operational risks.

## Recommendations
- Differentiated plans by use.
- Promotions for young and adult high-use users.
- Monitor outliers to identify key clients.
- Retention campaigns for medium-use users approaching their plan limits, for upselling.
- Flexible plans for high-use users with more GB and minutes, to support permanence and reduce churn.

## How to run
Open the `.ipynb` in Jupyter or Colab and run all cells.

---

## Versión en español

# Análisis de ConnectaTel

Análisis de clientes de telecomunicaciones para ConnectaTel en América Latina, con datos hasta 2024.

## Pregunta
Evaluar el comportamiento de los clientes para construir un perfil estadístico del cliente, detectar comportamientos atípicos, crear segmentos de clientes, identificar patrones de consumo, diseñar estrategias de retención y sugerir mejoras en los planes.

## Conjuntos de datos
- `plans.csv` — 2 planes, 8 columnas
- `users_latam.csv` — 4,000 usuarios, 8 columnas (edad, ciudad, fecha de registro, plan, fecha de baja)
- `usage.csv` — 40,000 registros, 6 columnas (llamadas y mensajes, fecha, duración/longitud)

Planes mostrados: Básico — 100 mensajes, 5 GB, 100 minutos, $12/mes. Premium — 500 mensajes, 20 GB, 600 minutos, $25/mes.

## Herramientas
Python, Pandas, NumPy, Seaborn, Matplotlib, Jupyter Notebook.

## Qué hice
Cargar y explorar los tres conjuntos de datos, limpiar los datos, construir una tabla `user_profile` con recuentos de mensajes, recuentos de llamadas y minutos de llamadas, segmentar a los clientes por uso y por edad, y visualizar los resultados.

Segmentos utilizados:
- Uso: Uso bajo (llamadas < 5 y mensajes < 5), Uso medio (llamadas < 10 y mensajes < 10), Uso alto (el resto)
- Edad: Joven (< 30), Adulto (30–59), Adulto mayor (≥ 60)

## Hallazgos clave
- Problemas de calidad de los datos encontrados: edad = -999, ciudad = "?", fechas futuras, y valores nulos en duración y longitud (5–20%).
- Los clientes jóvenes y adultos de alto uso son más activos en mensajes y llamadas.
- Clientes más valiosos identificados cualitativamente: clientes jóvenes y adultos de alto uso, con mayor potencial de fidelización.
- Valores atípicos: algunos usuarios con uso extremo, que pueden ser clientes estratégicos o riesgos operativos.

## Recomendaciones
- Planes diferenciados por uso.
- Promociones para usuarios jóvenes y adultos de alto uso.
- Monitorear los valores atípicos para identificar clientes clave.
- Campañas de retención para usuarios de uso medio que se acercan a los límites de su plan, para venta adicional (upselling).
- Planes flexibles para usuarios de alto uso con más GB y minutos, para favorecer la permanencia y reducir la baja (churn).

## Cómo ejecutar
Abrir el `.ipynb` en Jupyter o Colab y ejecutar todas las celdas.
