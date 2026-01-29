# 🔬 Test A/A/B y Optimización del Embudo en Aplicación Móvil

## 🎯 Objetivo de Negocio
Validar si un cambio de fuente propuesto por el equipo de producto impacta negativamente en la conversión de usuarios y, en paralelo, identificar cuellos de botella críticos dentro del embudo de conversión de una aplicación móvil de venta de alimentos.

---

## 💡 Resumen y Solución de Negocio

Este proyecto se centró en experimentación controlada (A/A/B Testing) y análisis de eventos para evaluar un cambio de diseño (tipografía) y entender el comportamiento de los usuarios a lo largo del funnel de conversión.
Además de validar estadísticamente el impacto del rediseño, se realizó un análisis profundo del embudo, permitiendo identificar oportunidades de optimización con alto potencial de impacto en ventas.

---

## 📊 Impacto y Conclusiones
## 🔄 Análisis del Embudo (Funnel)

Se mapeó el flujo de conversión del usuario desde el primer contacto hasta la compra, identificando caídas críticas en cada etapa:
| Fase del Funnel | Tasa de conversión | **Impacto** |
|------|------|------|
| MainScreenAppear → OffersScreenAppear | Baja (~40%) | Cuello de botella crítico. La mayor pérdida de usuarios ocurre aquí, lo que sugiere que las ofertas no son lo suficientemente atractivas o visibles desde la pantalla principal. |
| OffersScreenAppear → CartScreenAppear | Tasa de conversión: Moderada | Los usuarios que exploran ofertas avanzan de manera estable hacia el carrito. |
| CartScreenAppear → PaymentScreenAppear | Alta | El proceso de checkout es eficiente y no representa una fricción relevante. |

---

## 🧪 Resultados de la Prueba A/B (Cambio de Fuente)

Diseño Experimental:

- Grupo de prueba: ExpId 248
- Grupos de control: ExpId 246 y 247

## Método Estadístico:
Prueba Z para proporciones para evaluar diferencias en tasas de conversión.

## **Conclusión Estadística:**

**No se encontraron diferencias estadísticamente significativas entre el grupo de prueba (nueva fuente) y los grupos de control.**

---

## 📌 Recomendación Estratégica

**Aprobar el cambio de fuente: El rediseño no afecta negativamente las métricas clave y puede implementarse para mantener consistencia visual y de marca.**

**Priorizar futuros experimentos: Dirigir los próximos A/B Tests al principal cuello de botella (MainScreen → OffersScreen), donde existe el mayor potencial de incremento en conversión mediante mejoras en diseño, visibilidad o incentivos.**

---

## 🛠️ Stack Tecnológico

* **Lenguaje:** Python
* **Librerías Clave:** 'Pandas', 'NumPy', 'SciPy.stats', 'Matplotlib/Seaborn'

* **Metodología:** **Funnel Analysis**, **Análisis de Eventos**, **Pruebas de Hipótesis**, **Análisis de Frecuencia de Compra y Métricas de Producto.**
