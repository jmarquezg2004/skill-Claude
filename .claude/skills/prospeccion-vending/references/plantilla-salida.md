# Plantilla de salida (CSV)

Archivo: `prospectos/<AAAA-MM-DD>-<zona>-<segmento>.csv`

```
empresa,segmento,direccion,zona,personas_estimadas,horario,trafico_visitantes,solucion_cafe_actual,decisor_cargo,decisor_nombre,canal,contacto,score,categoria,gancho,siguiente_accion,fecha_accion,fuente,verificar
```

- `personas_estimadas`: número o rango + base (p. ej. "150–200 (LinkedIn)").
- `contacto`: solo datos corporativos públicos y verificados; si no, vacío.
- `gancho`: el dato real que se usará en el mensaje.
- `fuente`: URL o "visita" / "llamada".
- `verificar`: qué falta confirmar.

Si el usuario quiere CRM, estas columnas mapean directo a HubSpot / Pipedrive (Company, Contact, Deal stage = "Prospecto A/B/C").
