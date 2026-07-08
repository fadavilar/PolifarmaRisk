# PolifarmaRisk — Análisis de Polifarmacia

App web autocontenida (HTML/CSS/JS, sin build ni backend) para el análisis de riesgo de polifarmacia en pacientes crónicos pluripatológicos: interacciones medicamentosas, riesgo de adherencia y confusión de medicamentos (LASA).

Desarrollada para el Congreso Internacional de Investigaciones — UniNavarra.

## Usar

Abre `index.html` directamente en el navegador (funciona offline, sin instalación) o visita la versión publicada en GitHub Pages.

En el celular, puedes "Agregar a pantalla de inicio" desde el navegador para instalarla como si fuera una app.

## Contenido

- `index.html` — la aplicación completa (motor de riesgo, UI, datos clínicos).
- `cum-catalog.js` — catálogo de 11.299 registros vigentes (marca + principio activo, buscable por ambos), extraído del [Código Único de Medicamentos (CUM) — INVIMA, datos.gov.co](https://www.datos.gov.co/Salud-y-Protecci-n-Social/C-DIGO-NICO-DE-MEDICAMENTOS-VIGENTES/i7cb-raxc/about_data).
- `serve.ps1` — servidor HTTP estático mínimo (PowerShell) para probar la app localmente sin depender de Node/Python; úsalo con `powershell -File app/serve.ps1` y abre `http://localhost:8843/`.
- `manifest.json`, `icon.svg` — metadatos para instalación como app (PWA ligera).

## Fuentes clínicas

El motor de reglas cita su fuente en cada hallazgo. Ver la sección "Referencias y evidencia" dentro de la app para el detalle completo (STOPP/START v3, AGS Beers Criteria 2023, ISMP List of Confused Drug Names, OMS, NICE).

## Aviso

Herramienta con fines educativos y de demostración. No sustituye el criterio clínico ni bases de datos regulatorias.
