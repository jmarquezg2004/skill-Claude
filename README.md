# Agente de prospección — Subito Company

Agente de Claude Code + skill para prospectar clientes B2B de máquinas de café vending.

```
.claude/
  agents/prospector-subito.md          # el agente (SDR)
  skills/prospeccion-vending/
    SKILL.md                           # flujo de prospección
    references/perfil-empresa.md       # ← COMPLETAR primero
    references/icp-scoring.md          # segmentos, filtros, scoring A/B/C, decisores
    references/mensajes.md             # email, WhatsApp, llamada, LinkedIn, objeciones, cadencia
    references/plantilla-salida.md     # columnas del CSV
prospectos/                            # aquí se guardan las listas generadas
```

## Uso
1. Completa `references/perfil-empresa.md` (cobertura, modelo comercial, consumo mínimo).
2. En Claude Code, dentro de este repo:
   - `Usa el agente prospector-subito: 20 leads en <ciudad/zona>, segmentos call centers y clínicas`
   - `/prospeccion-vending redacta la cadencia para estos 5 leads A`
