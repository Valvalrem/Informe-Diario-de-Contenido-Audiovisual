# Informe-Diario-de-Contenido-Audiovisual
Tengo que recalcar que, antes de proceder con el proyecto: 
- El asistente "Modelo AI" fue hecho en su totalidad con "Gemini" en lugar de "OpenAi".
- Se usó "Notion" para su debida base de datos y "OpenWeather" para las búsquedas referentes al clima.
# Link de la Base de Datos (Notion): https://jolly-lathe-35e.notion.site/3e07a2db85ef8052a4accf5e826d0187?v=3e07a2db85ef807c96d4000c119388fb

El asistente automatizado en n8n cumple con las siguientes tareas en cada ejecución:

Disparo diario: Se activa de forma automática todas las mañanas mediante el nodo Schedule a las 8:00 AM.

Extracción de datos: Consulta la base de datos en Notion para obtener información sobre series, películas y/o animes. En base a eso crea una sinopsis para cada uno. Además recopila el clima actualizado a través de la herramienta meteorológica.

Redacción con IA: El nodo AI Agent (Gemini) genera las sinopsis de series e integra la información del tiempo, estructurando todo el informe en formato HTML con tarjetas visuales estilizadas.

Control Humano (Human-in-the-Loop): Envía un primer correo a tu bandeja de Gmail con una tarjeta de color y un botón de aprobación. En ese momento, el flujo entra en pausa mediante el nodo Wait.

Despacho definitivo: Una vez que haces clic en Aprobar y Enviar Briefing, la URL reactiva la secuencia y envía el boletín final estilizado al destinatario.
