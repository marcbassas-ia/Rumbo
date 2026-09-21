# Plan de validación de Nómada

Objetivo: saber, **antes de invertir**, si la idea engancha. No validamos la
tecnología (ya funciona), validamos la **demanda** y el **comportamiento**:
¿la gente quiere viajar barato con planes reales?, ¿aportaría y buscaría por precio?

## Qué medimos (2 señales)

1. **Demanda** — ¿les interesa lo suficiente para dejar su correo?
   - Métrica: nº de altas en la lista de espera (landing).
   - Señal buena: de cada 10 personas a las que se lo enseñas, **3+ se apuntan**.

2. **Comportamiento** — ¿usarían la comunidad de precios?
   - Métrica: al ver el prototipo, ¿publicarían su viaje?, ¿buscarían por precio?
   - Señal buena: **mayoría diría que sí** y al menos algunos lo hacen de verdad.

## Cómo hacerlo (barato y rápido, 1-2 semanas)

1. **Publica la landing** (`index.html`) en GitHub Pages → URL pública gratis.
2. **Enséñala a 15-20 personas** reales: amigos que viajan, compañeros, grupos
   de viajeros jóvenes, 1-2 foros/subreddits de viajes o mochileros, historias
   de Instagram. Texto de difusión abajo.
3. **A quien tenga interés**, enséñale el prototipo en vivo (tu pantalla o tu
   sesión de Claude) y observa su reacción con las preguntas de abajo.
4. **Anota** cada respuesta en una hoja simple (o Google Form).

## Preguntas para las entrevistas (5 minutos, sin dirigir)

Primero deja que lo use sin ayuda y observa. Luego pregunta:

1. ¿Cuándo fue tu último viaje y cómo lo planificaste? (dolor real)
2. ¿Qué es lo primero que miras al planear: sitios, o cuánto vas a gastar?
3. Del 1 al 10, ¿cuánto te ayudaría ver el **precio** de cada plan? ¿Por qué?
4. ¿Publicarías **tu** viaje con precios para que otros lo copien? ¿Qué te frena?
5. ¿Buscarías viajes filtrando por presupuesto? ¿Cuándo lo usarías?
6. Si esto existiera mañana, ¿lo usarías? ¿Pagarías algo? ¿Cuánto?
7. ¿Qué le falta o qué te ha sobrado?

> Regla de oro: escucha, no vendas. Un "qué chulo" no vale; vale un
> "me apunto", un "lo usaría para X", o que **de verdad** deje su correo.

## Criterios de decisión (honestos)

- **SEGUIR / invertir**: 3+ de cada 10 se apuntan Y la mayoría diría que
  publicaría o buscaría por precio. Hay señal → merece backend y marca en serio.
- **AJUSTAR**: interés en la herramienta pero nadie quiere aportar a la
  comunidad → el problema es el arranque de contenido; replantear el incentivo.
- **PIVOTAR**: casi nadie se apunta ni ve valor en el precio → el ángulo no
  conecta; cambiar de foco antes de gastar.

## Texto para difundir (copia y pega)

> Estoy montando **Nómada**, una web para planear viajes viendo **cuánto cuestan
> de verdad** y copiar itinerarios reales que otros ya han hecho, con sus precios.
> Pensado para viajar bien gastando poco. ¿Te interesaría? Déjame tu correo aquí
> y dime qué te parece: [URL de la landing]

## Publicar la landing en GitHub Pages (gratis)

1. En GitHub: repo **Rumbo** → Settings → Pages.
2. En "Build and deployment", Source: **Deploy from a branch**.
3. Branch: **main**, carpeta **/ (root)** → Save.
4. En 1-2 min tendrás la URL pública: `https://marcbassas-ia.github.io/Rumbo/`
   (servirá `index.html`, que es la landing).

### Capturar correos de verdad (opcional, gratis)
- Crea un formulario en https://formspree.io (gratis) y pega su endpoint en
  `FORM_ENDPOINT`, dentro de `index.html`. Si lo dejas vacío, el botón abre el
  correo del visitante como alternativa.
- Para opiniones: crea un Google Form con las preguntas de arriba y pega su
  enlace en `FEEDBACK_FORM_URL`.
