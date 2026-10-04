# Prototipo tecnológico 5S + RFID – Almacén de producto terminado

Aplicación web (HTML5, CSS y JavaScript) que demuestra el funcionamiento del prototipo 5S + RFID
para la ubicación, el control y el despacho oportuno de lotes de producto terminado en un almacén
de 7.00 m × 4.00 m de una empresa fabricante de envases de cartón ondulado.

## Módulos
1. **Base de pedidos (lotes):** registro manual, carga desde Excel (`Plantilla_Base_Lotes.xlsx`) y generador de demanda de prueba (4 a 7 lotes por día hábil).
2. **Simulación RFID:** emulador de lecturas (arco de entrada, tag de posición y arco de salida), reloj acelerado, plano 5S, alertas, semáforo e indicadores.
3. **Historial y alertas:** incidencias con tiempo sin corregir, filtros, exportación a Excel y avisos por correo (simulados).

## Cómo ejecutarlo
- **En línea:** publicado con GitHub Pages en `https://<usuario>.github.io/prototipo-5s-rfid/`.
- **Local:** descargar `index.html` y abrirlo con Chrome, Edge o Firefox (la carga/exportación de Excel requiere internet para la librería SheetJS).

## Datos
La base de lotes se guarda en el almacenamiento local del navegador (`localStorage`) del equipo donde se usa.
El botón **Restablecer ejemplo** vuelve al escenario de prueba de 51 lotes (semilla 7).

## Tecnologías
HTML5 · CSS · JavaScript (sin frameworks) · SVG (plano) · SheetJS 0.18.5 (lectura/escritura de Excel) · GitHub Pages (alojamiento).

## Limitaciones
Las lecturas RFID son generadas por un emulador y el envío de correos es simulado. Para la implementación
con hardware se requieren etiquetas UHF, dos arcos de lectura, Node-RED como puente con los lectores y un servidor de correo (SMTP).
