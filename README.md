# 📊⚠️Detección de Anomalías de Volumen No Confirmadas por Precio

## 📌Descripción del proyecto

Este proyecto implementa una consulta SQL para detectar anomalías en el volumen de negociación que no están acompañadas por movimientos de precio consistentes.

El objetivo es identificar situaciones donde el volumen aumenta de forma significativa, pero el precio no confirma el movimiento, lo que puede indicar:
- Distribución o acumulación encubierta
- Falta de convicción del mercado
- Señales tempranas de reversión
- Distorsiones o eventos atípicos

## 🎯Objetivos del proyecto

- Detectar incrementos anómalos de volumen.
- Evaluar la confirmación (o falta de ella) en el precio.
- Identificar divergencias precio-volumen.
- Automatizar análisis técnico avanzado mediante SQL.
- Generar alertas para análisis y toma de decisiones.

## 🏦Contexto financiero

En análisis técnico, el volumen debería confirmar al precio:
- Subas de precio con volumen creciente → movimiento saludable.
- Volumen elevado sin movimiento de precio → posible anomalía.

📌 La ausencia de confirmación suele anticipar:

- Cambios de tendencia
- Movimientos bruscos posteriores
- Reducción de liquidez real
- Señales falsas de mercado

Este análisis es clave para:
- Trading cuantitativo
- Research financiero
- Gestión de riesgo
- Detección temprana de anomalías

## 🧠Lógica del análisis

La consulta SQL:
- Calcula el volumen promedio histórico.
- Detecta picos de volumen fuera de rango.
- Evalúa la variación de precio en el mismo período.
- Identifica casos donde:
- Volumen ↑ significativamente
- Precio ≈ estable o sin confirmación
- Marca el evento como anomalía precio-volumen.

📌 Los umbrales y ventanas son configurables.

## 📊Ejemplos de anomalías detectadas

- Volumen inusualmente alto con precio lateral.
- Incrementos de volumen sin ruptura de soporte/resistencia.
- Actividad elevada previa a cambios bruscos.
- Divergencias persistentes en determinados activos.

## 🛠️Tecnologías utilizadas

SQL

Compatible con:
- PostgreSQL
- BigQuery
- SQL Server
- Oracle
- MySQL (con ajustes menores)

## 📁Estructura del proyecto

├── Anomalia_volumen_no_confirmada_por_precio.sql
└── README.md

## ▶️Cómo utilizar la consulta

Abrir el archivo Anomalia_volumen_no_confirmada_por_precio.sql.

Configurar:
- Tabla de precios y volumen
- Ventana temporal
- Umbrales de volumen y precio
- Ejecutar la consulta en el motor SQL.
- Analizar resultados o integrarlos en dashboards.

## 🚀Posibles extensiones

- Incorporar análisis por sector o mercado.
- Medir persistencia de la anomalía.
- Combinar con indicadores de volatilidad.
- Generar alertas automáticas.
- Integrar con modelos predictivos.

## 👤Autora

Flavia Hepp
Proyecto de SQL aplicado a análisis técnico y detección de anomalías financieras.

***
📊⚔️ **Mucho volumen… pero el precio no se mueve — esto no es ruido**

En trading, solemos asociar volumen alto con movimientos fuertes.

Pero hay días donde pasa algo mucho más interesante 👇

---

💡 **La anomalía: volumen extremo sin confirmación en precio**

* 🔥 Volumen 3x superior al promedio (30 días)
* ⚖️ Pero el precio prácticamente no se mueve (< 0.5%)

---

🧠 **¿Qué está pasando acá?**

No es falta de interés.
Es todo lo contrario.

👉 Es una **batalla intensa entre compradores y vendedores**

* Grandes órdenes enfrentadas
* Absorción de liquidez
* Posicionamiento institucional

---

🚨 **¿Por qué es importante?**

Porque estos momentos suelen ser **antesala de movimientos relevantes**:

* 📈 Breakout fuerte
* 📉 Caída abrupta
* 🔄 Cambio de tendencia

👉 El mercado está “cargando energía”

---

📊 ¿Cómo lo interpreto?

🔴 Si ocurre cerca de resistencias → posible distribución
🟢 Si ocurre en soportes → posible acumulación

---

⚡ Aplicaciones prácticas:

* Detectar zonas de alta tensión en el mercado
* Anticipar movimientos explosivos
* Mejorar timing de entrada/salida
* Evitar señales falsas basadas solo en volumen

---

💬 El precio te muestra el resultado…
👉 pero el volumen te muestra la pelea.

---

Y a veces, cuando nadie “gana” en el día…
es porque algo grande está por empezar.

¿Alguna vez viste una vela “quieta” con volumen gigante y después vino el movimiento fuerte? 👇

