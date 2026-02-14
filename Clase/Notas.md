## Notas – Trabajo en clase (Caso base: Clínica Salud Viva)

### ERD (borrador)
Entidades: Paciente, Cita, Médico, Especialidad, Factura.

Relaciones clave:
- Paciente 1:N Cita
- Médico 1:N Cita
- Especialidad 1:N Cita
- Cita 1:0..1 Factura

Decisiones de modelado:
- La cita referencia a Paciente, Médico y Especialidad con claves foráneas.
- La factura referencia a Cita (única) para representar 1 factura por cita (opcional).

### Diagrama de contexto (borrador)
Actores: Paciente, Médico, Asistente/Recepción.
Sistemas: Agendamiento, Notificador (SMS/Email), ERP.
Flujos principales: solicitud, confirmación, disponibilidad, reprogramación y datos para registro/facturación.
