# Abogados La Rioja — Presupuestador de Honorarios

Calculadora de honorarios profesionales basada en el **Decreto-Ley 4170/82 de La Rioja**
(texto ordenado por Ley 5827). Pensada para que cualquier abogado matriculado en la
provincia cargue los datos de una causa puntual y obtenga, en segundos, el honorario
mínimo según la escala legal vigente.

**Demo en vivo:** https://honorariosabogados.github.io/presupuestador-4170/
*(reemplazá esta línea por la URL real una vez que actives GitHub Pages)*

## Qué resuelve

- **Con monto (Art. 6-31):** juicios con reclamo económico — aplica el porcentaje de
  escala (10-20%), el tipo de trámite (ejecutivo, cautelar, allanamiento, etc.) y el
  piso legal de 10 jus.
- **Sin monto (Art. 15.A):** divorcios, adopciones, tenencia y otros asuntos con jus
  fijo.
- **Penal:** defensas por sumario y plenario, excarcelación, eximición de prisión,
  particular damnificado y querella — todos los valores en jus según el artículo que
  corresponde.
- **Extrajudicial (Art. 15.B):** consultas, redacción de contratos y demás labor fuera
  de juicio.

Además de la escala legal, incluye un **ajuste por complejidad** (a pactar con el
cliente, no forma parte de la ley) y un botón para copiar el presupuesto ya armado.

## Cómo está hecho

Un único front-end en HTML, CSS y JavaScript, sin backend ni dependencias de build.
Funciona como **PWA instalable**: se puede agregar a la pantalla de inicio desde
Chrome (Android/escritorio) o desde el menú Compartir en iPhone, y sigue funcionando
sin conexión gracias al `service-worker.js`. Cada vez que hay internet, busca sola la
versión más nueva publicada acá — no hace falta reinstalarla para recibir cambios.

## Actualizar el valor del jus

El valor vigente está fijo en el código, no es editable desde la app (para que sea el
mismo número para todos). Para actualizarlo:

1. Abrí `index.html` y buscá la constante `VALOR_JUS` al inicio del `<script>`.
2. Cambiá el número por el valor vigente.
3. Subí el archivo actualizado pisando el anterior (`Add file → Upload files`).

Todos los que ya tengan la app instalada van a ver el nuevo valor la próxima vez que
la abran con conexión.

## Alcance y responsabilidad

Esta herramienta da el **piso legal orientativo** según la escala de la Ley 4170. El
honorario judicial definitivo lo fija el juez con las pautas del art. 5° (monto,
complejidad, mérito, trascendencia, etc.). No reemplaza el criterio profesional de
cada abogado en cada causa.

## Créditos

Desarrollado por **[@ab.geracaceres](https://instagram.com/ab.geracaceres)** para los
colegas de La Rioja. Se agradece mantener este crédito si se comparte o reutiliza.
