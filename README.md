# Granja Dorada - Sistema de Reposición de Bolsas

Autora: Blanco Milagros - UTN FRSN
Tablero Ágil: https://github.com/users/blancomilagros429-tech/projects/1/views/1

1. BPMN
Diagrama de reposición en `docs/Granja_Dorada_BPMN.bpmn` y `docs/BPMN.png`

2. Historias de Usuario (Tablero)
- HU1 - Envasado: descuento automático
- HU2 - Sistema: alerta stock mínimo  
- HU3 - Compras: definir cantidad
- HU4 - Depósito: registrar ingreso lote

3. Indicadores (KPIs)
- **KPI1 - % Roturas de stock:** (días con quiebre / días totales) * 100 | Meta <2%
- **KPI2 - Tiempo de reposición:** Horas desde alerta hasta ingreso | Meta <24h
- **KPI3 - Exactitud de inventario:** (stock sistema vs real) | Meta >98%

4. Uso de IA
- Herramienta: Meta AI
- Prompts utilizados: "ayudame a estructurar BPMN de reposición de bolsas", "definir HUs para sistema de stock"
- Validación humana: Revisión del flujo con operarios de Envasado y Depósito de Granja Dorada.

5. Git Flow
- Rama feature/entrega-4-bpmn -> PR #1 -> merge a main (evidencia en Pull Requests)
