# Rumbo · Planificador de viajes con IA

Prototipo de una web que genera itinerarios de viaje día a día con IA.
El usuario indica destino, fechas, personas, con quién viaja, intereses,
imprescindibles y (opcional) horas de llegada/salida y alojamiento; Claude
devuelve un plan con qué ver, dónde comer y cómo organizar los días.

## Funciones actuales
- Generación del itinerario con IA (capacidad `sample` de Claude Artifacts).
- Cualquier destino del mundo.
- Ajuste por hora de llegada/salida del transporte.
- Optimización de los días por cercanía al alojamiento.
- **Imprescindibles**: sitios/restaurantes que se incluyen sí o sí.
- Idioma ES / EN (interfaz e itinerario).
- Descargar y compartir el itinerario.
- **Comunidad**: publicar tu viaje y que otros lo copien y editen (capacidad `db`).
- Enlaces afiliado-ready a Booking, Airbnb y alquiler de coche
  (config `AFF` al inicio del `<script>` en `planner.html`).

## ⚠️ Importante sobre cómo se ejecuta
`planner.html` está pensado para ejecutarse **como Artifact de Claude**
(claude.ai). Usa el runtime de Claude (`window.claude` / `claude.use(...)`)
para la IA, la base de datos de la comunidad y las descargas.

Si abres el archivo como web estática normal (GitHub Pages, doble clic),
**esas funciones no se ejecutan** (no hay motor detrás). Este repo sirve para
**versionar el código**. Para tenerlo funcionando fuera de claude.ai haría
falta un backend propio (una API de IA + base de datos).

Artifact en vivo: https://claude.ai/artifact/5Y3tqqP6sJAmmL5sN8KEMW

## Monetización (modelo de negocio)
- Afiliación de viajes (Booking / Airbnb / coche) — comisión por reserva.
- Freemium: plan básico gratis, versión completa/PDF de pago.

## Pendiente / próximos pasos
- Editor manual del itinerario (arrastrar/reescribir a mano).
- Comunidad pública real (backend propio, hoy es interna de la organización).
- Alta en programas de afiliados y pegar los IDs en la config `AFF`.
