🔬 Test A/A/B y Optimización del Embudo en Aplicación Móvil

Visión General y Problema de Negocio
Este proyecto se centra en la experimentación (A/B Testing) y el análisis de eventos para una startup de venta de alimentos. El objetivo principal fue validar un cambio de fuente (diseño) propuesto por el equipo de producto y, al mismo tiempo, analizar el embudo de conversión de los usuarios.

El análisis busca responder:

¿El cambio de fuente impactó negativamente en la conversión de usuarios? (Prueba A/B)

¿Cuáles son los cuellos de botella (bottlenecks) más críticos en el funnel de la aplicación?

Objetivos del Análisis y Conclusiones Clave
1. Análisis del Embudo (Funnel)
Se mapeó el flujo de conversión del usuario desde el primer contacto hasta la compra, identificando caídas críticas en cada etapa.

Etapa del Funnel	Tasa de Conversión (Aproximada)	Impacto
MainScreenAppear → OffersScreenAppear	Baja (Aproximadamente 40%)	Cuello de Botella Crítico. La mayor caída de usuarios, indicando que las ofertas no son lo suficientemente atractivas o accesibles desde la pantalla principal.
OffersScreenAppear → CartScreenAppear	Moderada	Los usuarios que ven ofertas se convierten a carrito de manera estable.
CartScreenAppear → PaymentScreenAppear	Alta	La tasa de pago desde el carrito es alta, lo que indica que el proceso de checkout funciona bien.

2. Resultados de la Prueba A/B (Cambio de Fuente)
La prueba comparó un Grupo de Prueba (ExpId 248) con dos grupos de control (246 y 247).

Método: Se utilizó la Prueba Z para Proporciones para determinar la significancia estadística de la diferencia en las tasas de conversión entre los grupos.

Conclusión Estadística: No se encontraron diferencias estadísticamente significativas entre el grupo de prueba (fuente nueva) y los grupos de control.

Recomendación Estratégica para el Negocio
El análisis permitió ir más allá de la prueba A/B inicial para ofrecer una estrategia de producto:

Aprobar el Cambio de Fuente: Dado que el nuevo diseño no perjudica las métricas clave, se recomienda implementarlo para mantener la consistencia de marca.

Enfocar Próximos Experimentos: La inversión en futuros A/B Tests debe dirigirse a resolver el cuello de botella crítico (MainScreen a OffersScreen), ya que es el punto con mayor potencial para aumentar las ventas. Se sugiere experimentar con incentivos, diseño o visibilidad de las ofertas.

🛠️ Stack Tecnológico
Herramienta	Aplicación
Python (Pandas, NumPy)	Limpieza, manipulación y agregación de datos de eventos.
SciPy.stats	Aplicación de la Prueba Z para la Inferencia Estadística y cálculo del p-valor.
Matplotlib / Seaborn	Visualización del Funnel y las diferencias de conversión entre grupos.
Metodología	Funnel Analysis, Análisis de Eventos, Pruebas de Hipótesis.
---

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python
* **Librerías Clave:** `Pandas`, `Matplotlib/Seaborn` (Análisis de Frecuencia).
* **Metodología:** **Análisis de Frecuencia de Compra**, Agregación de Datos para Métricas de Producto, Exploración de Patrones de Comportamiento.
