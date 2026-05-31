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


 Se agrago al sulucion en python para el siguiente problema de pilas y colas:

 El Banco de Colombia está interesado en medir el desempeño de sus cajeros durante las operaciones de pagos y retiros, pues no cuenta con cajeros electrónicos y considera conveniente tener cajas disponibles para que los ciudadanos realicen sus operaciones sin demora. El banco desea saber si debe asignar una caja exclusiva para retiros y dos para pagos, o viceversa, esto con el propósito de adoptar las adecuaciones necesarias en miras de prestar el mejor servicio posible a sus usuarios.

Para resolver este caso, presta atención a la siguiente información:

El banco dispone de tres cajas para ambas finalidades (pagos y retiros), las cuales prestan su servicio de acuerdo con el tipo de usuario.  

En la Tabla 1 se definen los tipos de usuario, detallando los tiempos de llegada y servicio estimados para cada uno con base en la acción que deseen realizar. Ten en cuenta que el 70 % de los usuarios hace retiros, mientras que los demás realizan consignaciones o pagos. 

Por otro lado, los cajeros se deben simular como modelos M/M/1, pues son independientes. Además, se asume que la velocidad de atención es igual para todos los cajeros (inmediata) y la velocidad de desplazamiento es despreciable.  

El banco opera 8 horas al día. Se puede asumir que los días son iguales y establecer las sugerencias necesarias a partir de la modelación de un solo día y sus réplicas.

Ejecuta al menos 10 corridas del modelo y calcula las estadísticas necesarias para resolver los siguientes puntos:

Calcula las estadísticas necesarias para identificar el cajero con menor y mayor tiempo promedio de atención (no es necesario segregar los usuarios).

Establece el promedio de usuarios de cada tipo en la totalidad de cajeros.

Determina el total de usuarios de cada tipo en cada una de las réplicas y detalla el modelo con menor cantidad de usuarios por tipo.

Define si es necesario crear un nuevo cajero utilizando los tiempos promedio de espera en todos los criterios del modelo.

Decide cuántos cajeros deben ofrecer atención exclusiva para pagos y cuántos para retiros.

Los detalles de atención de cada cajero y servicio se definen a continuación:
Tipo de acción	Tipo de usuario	Exponencial de uso del servicio	Exponencial de media de llegada
Retiro	Rápido	1 minutos	1 minutos
	Normal	2 minutos	2 minutos
	Lento	3 minutos	3 minutos
	Muy lento	4 minutos	3 minutos
Consignación o pago	Rápido	3 minutos	1 minutos
	Normal	3 minutos	2 minutos
	Lento	5 minutos	3 minutos
	Muy lento	7 minutos	4 minutos
Las probabilidades de los tipos de usuario se detallan en la siguiente tabla:

Tipo de acción	Tipo de usuario	Probabilidad
Retiro	Rápido	0,23
	Normal	0,40
	Lento	0,17
	Muy lento	0,20
Consignación o pago	Rápido	0,10
	Normal	0,20
	Lento	0,30
	Muy lento	0,40


