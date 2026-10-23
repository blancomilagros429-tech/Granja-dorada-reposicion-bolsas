# Granja Dorada - Sistema de Reposición de Bolsas - Entrega 4

Repositorio Público: https://github.com/blancomilagros429-tech/Granja-dorada-reposicion-bolsas
Tablero Ágil (GitHub Projects):

Integrante
Blasco Milagros - Organización Empresarial - UTN

1. Descripción del Sistema
Sistema que automatiza el proceso de reposición de bolsas para envasado de Granja Dorada. Participan: Envasado/Depósito, Sistema de Stock automatizado, sector Compras y actor externo Proveedor de bolsas.

2. Modelado BPMN 2.0
El proceso modelado contempla el ciclo completo desde el retiro de bolsas hasta la reposición:
- **Pool Granja Dorada:** Lanes Envasado/Depósito, Sistema de Stock, Compras.
- **Pool Proveedor de bolsas:** actor externo.
- Flujo con control de stock mínimo, generación de alerta automática y reclamo por evento temporizador.
- Compuertas: ¿Stock actual <= stock mínimo?, ¿Pedido aprobado?, ¿Llega el pedido en X días?

3. Mecanismos de Control y Estándares de Desempeño
Indicadores para auditoría técnica:
- Stock mínimo respetado: Alerta generada si stock actual < stock mínimo
- Tiempo de respuesta de proveedor: X días (controlado por evento temporizador)
- Trazabilidad: registro de consumo, ingreso y actualización de stock
- % de pedidos completados a tiempo
- Estándares: Notación BPMN 2.0, commits descriptivos, Pull Request con revisión de pares

4. Declaración de Uso de IA
Este trabajo utilizó asistentes de IA para:
- Prompt 1: "Ayudame a mejorar la redacción del flujo de reposición de bolsas con eventos de mensaje"
- Prompt 2: "Generar 3 historias de usuario en formato Como/quiero/para para un sistema de stock de bolsas"
- Prompt 3: "Estructurar un README que cumpla con consignas de Organización Empresarial UTN punto 4"

Correcciones humanas efectuadas: Se validó la lógica de negocio real de Granja Dorada, se corrigió la posición de los gateways y mensajes de alerta a Compras, y se verificó que el pool Proveedor esté separado como actor externo según bibliografía de la cátedra.
