# Análisis del embudo de conversión y experimento A/A/B

Proyecto de análisis de datos enfocado en estudiar el comportamiento de los usuarios de una aplicación de productos alimenticios, analizar su embudo de conversión y evaluar mediante un experimento A/A/B el efecto de un cambio en el diseño de la aplicación.

## Objetivo

Analizar el comportamiento de los usuarios dentro de la aplicación para:

- Identificar las principales etapas del proceso de compra.
- Analizar la conversión entre las diferentes etapas del embudo.
- Detectar los puntos donde se produce la mayor pérdida de usuarios.
- Evaluar mediante un experimento A/A/B si un cambio en las fuentes tipográficas afecta el comportamiento y la conversión de los usuarios.

## Herramientas utilizadas

- Python
- Pandas
- Matplotlib
- Seaborn
- SciPy
- Statsmodels
- Jupyter Notebook

## Proceso de análisis

El proyecto incluye:

1. Importación y exploración inicial de los datos.
2. Limpieza y preparación del dataset.
3. Análisis exploratorio y selección del periodo de estudio.
4. Análisis del comportamiento de los usuarios.
5. Construcción y análisis del embudo de conversión.
6. Identificación de las principales pérdidas de usuarios entre etapas.
7. Validación de la asignación de usuarios a los grupos experimentales.
8. Análisis del experimento A/A/B.
9. Pruebas Z para comparar proporciones entre los grupos.
10. Corrección de Bonferroni para controlar el riesgo de falsos positivos en comparaciones múltiples.

## Principales resultados

El análisis del embudo mostró que:

- Se analizaron 7,534 usuarios dentro del periodo seleccionado.
- La principal pérdida de usuarios ocurre entre la pantalla principal y la pantalla de ofertas.
- La retención entre estas dos etapas es de aproximadamente 61.91%, lo que representa una pérdida cercana al 38.09%.
- La retención entre la pantalla de ofertas y el carrito es de aproximadamente 81.30%.
- La retención entre el carrito y el pago alcanza aproximadamente 94.78%.
- Aproximadamente el 47.70% de los usuarios que ingresan a la pantalla principal completan el proceso hasta el pago.

## Experimento A/A/B

Los usuarios fueron divididos en tres grupos experimentales:

- 246: grupo de control.
- 247: grupo de control.
- 248: grupo con las nuevas fuentes tipográficas.

La comparación A/A entre los grupos de control no mostró diferencias estadísticamente significativas en los eventos analizados.

Posteriormente, las comparaciones entre el grupo experimental y los grupos de control tampoco mostraron diferencias estadísticamente significativas.

En total se realizaron 20 pruebas de hipótesis. Para controlar el riesgo de falsos positivos asociado a comparaciones múltiples, se aplicó la corrección de Bonferroni, ajustando el nivel de significación de 0.05 a 0.0025.

Las conclusiones del experimento se mantuvieron después de aplicar esta corrección.

## Conclusión

Los resultados no proporcionan evidencia estadística de que el cambio de fuentes tipográficas genere diferencias significativas en el comportamiento o en la conversión de los usuarios.

Desde una perspectiva de negocio, el principal punto de mejora identificado se encuentra en la transición entre la pantalla principal y la pantalla de ofertas, donde se concentra la mayor pérdida de usuarios del embudo.

## Archivos

- `proyecto_sprint_12.ipynb`: notebook principal con el análisis completo.
- `logs_exp_us.csv`: dataset utilizado para el análisis de eventos y el experimento A/A/B.
- `requirements.txt`: dependencias de Python necesarias para ejecutar el proyecto.

## Instalación de dependencias

Para instalar las librerías necesarias:

```bash
pip install -r requirements.txt