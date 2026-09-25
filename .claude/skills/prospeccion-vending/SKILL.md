---
name: prospeccion-vending
description: Prospección B2B de clientes para Subito Company (máquinas de café vending). Úsalo cuando haya que encontrar, calificar, priorizar o contactar empresas/instituciones donde colocar máquinas de café — oficinas, hospitales, universidades, gimnasios, concesionarios, fábricas, hoteles, coworkings. Cubre búsqueda de leads por zona, scoring, identificación del decisor, mensajes de primer contacto (email, WhatsApp, llamada, LinkedIn), manejo de objeciones y seguimiento.
---

# Prospección Subito Company — Coffee Vending

Objetivo: llenar el pipeline con ubicaciones **rentables** (no solo "interesadas"). Una máquina mal ubicada cuesta ruta, reposición y mantenimiento sin volumen. Calificar duro antes de contactar.

## Antes de empezar

1. Lee `references/perfil-empresa.md`. Si tiene campos `[COMPLETAR]` críticos (zona de cobertura, modelo comercial, mínimo de consumo), pregúntale al usuario solo esos y sigue.
2. Confirma el input de la tarea: **zona** (ciudad/barrios/radio), **segmento(s)** y **cantidad** de leads. Si falta, usa por defecto: zona = cobertura del perfil, segmentos = top 3 del ICP, 20 leads.

## Flujo

### 1. Buscar
- Usa WebSearch / WebFetch si están disponibles: Google Maps, directorios empresariales, LinkedIn (páginas de empresa), cámaras de comercio, listados de parques empresariales, rankings locales de empleadores.
- Consultas útiles: `"<segmento>" "<ciudad>"`, `"parque empresarial" "<ciudad>"`, `"call center" <ciudad> empleados`, `"clínica" OR "hospital" <barrio>`.
- **Nunca inventes** empresas, teléfonos, emails ni nombres de personas. Si un dato no está verificado, déjalo vacío y marca `fuente` / `verificar`.

### 2. Calificar (scoring)
Aplica `references/icp-scoring.md`. Cada lead sale con puntaje 0–100 y categoría A/B/C. Descarta (D) lo que no pase los filtros eliminatorios.

### 3. Identificar decisor
Según tamaño del lugar (ver tabla en `references/icp-scoring.md`): Office manager / Administración / Servicios generales / Compras / RR.HH. (bienestar) / Gerente de sede. Dueño en negocios pequeños.

### 4. Redactar primer contacto
Usa `references/mensajes.md`. Personaliza con **un gancho real** del lead (nº de empleados, turnos 24/7, sala de espera, apertura de sede nueva). Nada genérico.

### 5. Entregar
Guarda en `prospectos/<fecha>-<zona>-<segmento>.csv` con las columnas de `references/plantilla-salida.md` y muestra un resumen:
- Top 5 leads A con por qué.
- Siguiente acción concreta por lead (quién, canal, cuándo).
- Huecos de información que conviene verificar por teléfono/visita.

## Reglas
- Calidad > volumen. 10 leads A valen más que 50 C.
- Prioriza densidad geográfica: leads cerca entre sí abaratan la ruta de reposición.
- Respeta leyes anti-spam y de protección de datos del país: contacto B2B, emails corporativos, opción de baja, sin scraping de datos personales sensibles.
- Si el usuario pide seguimiento, usa la cadencia de `references/mensajes.md` (5 toques en 14 días).
