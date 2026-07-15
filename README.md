# Rúbrica de Evaluación — Creación de Empresa MADSI

Formulario de evaluación para la opción de grado **Creación de Empresa** de la Maestría en Análisis de Datos y Sistemas Inteligentes (MADSI) — Universidad Santo Tomás, Bucaramanga.

## Descripción

Aplicación web estática servida con Node.js/Express, desplegada en Railway. Permite a los evaluadores diligenciar la rúbrica de evaluación por capítulos, generar un PDF firmado y enviar la calificación al sistema de seguimiento MADSI.

## Criterios de evaluación

| # | Capítulo | Peso |
|---|---|---|
| 1 | Introducción y Contextualización | 10% |
| 2 | Problema, Oportunidad y Propuesta de Valor | 25% |
| 3 | Estudio de Mercado y Modelo de Negocio | 25% |
| 4 | Estructura Organizacional y Viabilidad | 30% |
| 5 | Conclusiones y Proyección | 10% |

**Concepto:** Aprobado (≥ 4.5) / Aprobado con correcciones (3.5–4.4) / Reprobado (< 3.5)

## Uso

El enlace se envía a cada evaluador con parámetros de proyecto y evaluador:

```
https://<dominio>.up.railway.app/rubrica_creacion_empresa.html?proyecto=ID&evaluador=1
```

- `proyecto`: ID del proyecto en el sistema de seguimiento
- `evaluador`: `1` = Evaluador 1 / `2` = Evaluador 2

## Stack

- HTML + CSS + JavaScript (sin frameworks)
- [jsPDF](https://github.com/parallax/jsPDF) para generación de PDF en cliente
- Node.js + Express para servidor estático
- Railway para despliegue
- Backend: [madsi-seguimiento](https://github.com/chvn00/madsi-seguimiento)

## Archivos

```
rubrica_creacion_empresa.html   # Formulario principal
server.js                       # Servidor Express
package.json
logo_usta.png                   # Logo institucional
```
