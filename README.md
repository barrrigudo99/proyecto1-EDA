
#  **Introducción**

En este notebook realizamos un **proceso completo de análisis de datos** aplicado a un dataset real con estadísticas de jugadores pertenecientes a las **cinco grandes ligas europeas** durante la temporada **2023-2024**.

El objetivo general es **limpiar, transformar, explorar y visualizar** la información para obtener conclusiones relevantes sobre el rendimiento de los jugadores, tanto a nivel global como por ligas y equipos específicos. A lo largo del documento se incluye un análisis detallado del Real Madrid y posteriormente un estudio comparativo para todos los equipos de **La Liga**.

---

##  **1. Carga y limpieza del dataset**

En esta primera fase se realiza la importación del archivo `big_5_players_stats_2023_2024.csv`, seguida de una limpieza exhaustiva de los datos:

- Conversión de columnas numéricas (enteros y decimales) a sus tipos correctos.  
- Identificación y corrección de valores no válidos.  
- Eliminación de duplicados.  
- Homogeneización de columnas tipo string, enteros y floats.

Este paso es esencial para garantizar que los análisis posteriores se basen en un dataset íntegro y estructurado correctamente.

---

##  **2. Análisis exploratorio de datos (EDA)**

Se realiza una exploración inicial para comprender la estructura y características principales del dataset:

- **Conteo de jugadores por liga.**
- **Distribución de edades** mediante gráficos de barras, histogramas, boxplots, violin plots y heatmaps.
- Uso de **frecuencia absoluta y relativa** para interpretar proporciones entre ligas.

Este análisis permite identificar tendencias globales como:

- rangos de edad predominantes,
- diferencias entre competiciones,
- presencia de valores atípicos.

---

##  **3. Análisis focalizado en el Real Madrid**

Se lleva a cabo un estudio específico sobre los jugadores del Real Madrid con distintos enfoques:

- Goles totales por jugador.  
- Goles por minuto jugado (eficiencia real).  
- xG (goles esperados) por jugador.  
- Comparación visual entre rendimiento real y rendimiento esperado mediante barras superpuestas.

Este análisis permite identificar:

- jugadores altamente eficientes,
- jugadores que generan ocasiones pero marcan menos,
- y el comportamiento ofensivo por minuto comparado con el xG.

---

##  **4. Extensión del análisis a todos los equipos de La Liga**

Se replica el mismo procedimiento para cada equipo de la liga española:

- Cálculo de métricas avanzadas (goles/min, xG/min).  
- Ordenación de jugadores por eficiencia.  
- Visualización comparativa por equipo.

Esto permite observar diferencias en eficiencia ofensiva y rendimiento relativo dentro de cada plantilla de La Liga.

---

##  **5. Visualizaciones avanzadas: Eficiencia Real vs Esperada**

Finalmente, se construye un gráfico global de dispersión (scatter plot) para representar **a todos los jugadores de La Liga en conjunto**:

- **Eje X:** xG (goles esperados) por minuto.  
- **Eje Y:** goles por minuto.  
- **Color:** diferencia entre goles y xG (sobrerendimiento vs subrendimiento).  
- **Tamaño:** minutos jugados (impacto real del jugador).

Este tipo de visualización permite identificar patrones como:

- jugadores que rinden por encima de lo esperado,  
- jugadores que subrinden pese a generar peligro,  
- tendencia general de la competición.

Además, se introduce un **filtro de minutos mínimos (600 min)** para eliminar ruido estadístico y centrarse únicamente en jugadores con participación significativa. La comparación entre el gráfico sin filtro y el filtrado permite observar cómo la eficiencia se vuelve más coherente cuando se excluyen futbolistas con escasa participación.

---

##  **6. Conclusión general**

A través del análisis desarrollado en este notebook se consigue:

- Conocer la distribución y características principales del dataset.  
- Estudiar las diferencias entre ligas y equipos.  
- Evaluar la eficiencia ofensiva de jugadores mediante métricas reales y avanzadas.  
- Identificar casos de sobrerendimiento y subrendimiento respecto al xG.  
- Mejorar la calidad del análisis mediante filtros apropiados (p. ej., minutos mínimos).  

De esta manera, el estudio permite obtener una visión completa, sólida y fundamentada del rendimiento de los jugadores en las cinco grandes ligas europeas durante la temporada 2023-2024.




#  **Introducción**

En este notebook realizamos un **proceso completo de análisis de datos** aplicado a un dataset real con estadísticas de jugadores pertenecientes a las **cinco grandes ligas europeas** durante la temporada **2023-2024**.

El objetivo general es **limpiar, transformar, explorar y visualizar** la información para obtener conclusiones relevantes sobre el rendimiento de los jugadores, tanto a nivel global como por ligas y equipos específicos. A lo largo del documento se incluye un análisis detallado del Real Madrid y posteriormente un estudio comparativo para todos los equipos de **La Liga**.

---

##  **1. Carga y limpieza del dataset**

En esta primera fase se realiza la importación del archivo `big_5_players_stats_2023_2024.csv`, seguida de una limpieza exhaustiva de los datos:

- Conversión de columnas numéricas (enteros y decimales) a sus tipos correctos.  
- Identificación y corrección de valores no válidos.  
- Eliminación de duplicados.  
- Homogeneización de columnas tipo string, enteros y floats.

Este paso es esencial para garantizar que los análisis posteriores se basen en un dataset íntegro y estructurado correctamente.

---

##  **2. Análisis exploratorio de datos (EDA)**

Se realiza una exploración inicial para comprender la estructura y características principales del dataset:

- **Conteo de jugadores por liga.**
- **Distribución de edades** mediante gráficos de barras, histogramas, boxplots, violin plots y heatmaps.
- Uso de **frecuencia absoluta y relativa** para interpretar proporciones entre ligas.

Este análisis permite identificar tendencias globales como:

- rangos de edad predominantes,
- diferencias entre competiciones,
- presencia de valores atípicos.

---

##  **3. Análisis focalizado en el Real Madrid**

Se lleva a cabo un estudio específico sobre los jugadores del Real Madrid con distintos enfoques:

- Goles totales por jugador.  
- Goles por minuto jugado (eficiencia real).  
- xG (goles esperados) por jugador.  
- Comparación visual entre rendimiento real y rendimiento esperado mediante barras superpuestas.

Este análisis permite identificar:

- jugadores altamente eficientes,
- jugadores que generan ocasiones pero marcan menos,
- y el comportamiento ofensivo por minuto comparado con el xG.

---

##  **4. Extensión del análisis a todos los equipos de La Liga**

Se replica el mismo procedimiento para cada equipo de la liga española:

- Cálculo de métricas avanzadas (goles/min, xG/min).  
- Ordenación de jugadores por eficiencia.  
- Visualización comparativa por equipo.

Esto permite observar diferencias en eficiencia ofensiva y rendimiento relativo dentro de cada plantilla de La Liga.

---

##  **5. Visualizaciones avanzadas: Eficiencia Real vs Esperada**

Finalmente, se construye un gráfico global de dispersión (scatter plot) para representar **a todos los jugadores de La Liga en conjunto**:

- **Eje X:** xG (goles esperados) por minuto.  
- **Eje Y:** goles por minuto.  
- **Color:** diferencia entre goles y xG (sobrerendimiento vs subrendimiento).  
- **Tamaño:** minutos jugados (impacto real del jugador).

Este tipo de visualización permite identificar patrones como:

- jugadores que rinden por encima de lo esperado,  
- jugadores que subrinden pese a generar peligro,  
- tendencia general de la competición.

Además, se introduce un **filtro de minutos mínimos (600 min)** para eliminar ruido estadístico y centrarse únicamente en jugadores con participación significativa. La comparación entre el gráfico sin filtro y el filtrado permite observar cómo la eficiencia se vuelve más coherente cuando se excluyen futbolistas con escasa participación.

---

##  **6. Conclusión general**

A través del análisis desarrollado en este notebook se consigue:

- Conocer la distribución y características principales del dataset.  
- Estudiar las diferencias entre ligas y equipos.  
- Evaluar la eficiencia ofensiva de jugadores mediante métricas reales y avanzadas.  
- Identificar casos de sobrerendimiento y subrendimiento respecto al xG.  
- Mejorar la calidad del análisis mediante filtros apropiados (p. ej., minutos mínimos).  

De esta manera, el estudio permite obtener una visión completa, sólida y fundamentada del rendimiento de los jugadores en las cinco grandes ligas europeas durante la temporada 2023-2024.



