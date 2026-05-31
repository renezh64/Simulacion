Simulacion de Yatzee por metodo montecarlo
El siguiente codigo en python simula el juego yatzee usando metodo montecarlo.

Y el segundo cuaderno de colab desmuetra el proceso de implemetacion de cadenas me marcok ocultas donde se immplemento el algoritmo de viterbi para entrar el estado mas probable (multiplicacion del todos los estados buscando el valor max alto),
el problema de predicción del estado del trafico vehicular basándose en velocidades promedio observadas, con las siguientes especificacionesbasándose en velocidades promedio observadas, con las siguientes especificaciones:
Estados ocultos: 'Tráfico Fluido', 'Tráfico Moderado', 'Tráfico Congestionado'
Observaciones: 'Velocidad Alta', 'Velocidad Media', 'Velocidad Baja'
Con la siguiente matriz de transición:
	Fluido	Moderado	Congestionado
Fluido	0.7	0.25	0.05
Moderado	0.3	0.5	0.2
Congestionado	0.1	0.4	0.5
Matriz de emisión:
	Alta	Media	Baja
Fluido	0.8	0.15	0.05
Moderado	0.2	0.6	0.2
Congestionado	0.05	0.25	0.7
Distribución inicial: Fluido: 0.5 , Moderado: 0.3 , congestionado: 0.2
Donde se simula 48 mediciones  (un dia completo, cada 30), se generaron velocidades reales km/h (Alta: 80-100, Media: 40-80, Baja: 0-40)
Se calcula métricas de transporte:
   - Horas pico identificadas
   - Tiempo promedio en congestión
   - Velocidad promedio por estado
   - Índice de congestión (0-100)
Se predice tráfico para las próximas horas
Identificar patrones: ¿cuándo es más probable la congestión?
Generar rutas alternativas sugeridas durante congestión
Incluir análisis de impacto ambiental (emisiones en congestión)
 