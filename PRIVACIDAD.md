# Cómo trata Bidea tus datos

_Última actualización: 6 de noviembre de 2026 (versión 0.63 y versión web para iPhone)_

Bidea es una app gratuita, sin anuncios, hecha por una persona particular. Este texto explica en lenguaje sencillo qué datos guarda, para qué y cómo borrarlos.

## Quién es responsable

Bidea la mantiene a título personal el titular del repositorio [github.com/Marke12/bidea-releases](https://github.com/Marke12/bidea-releases). Para cualquier duda sobre tus datos, o para pedir que los veamos, corrijamos o borremos, escribe a **[gaaapla7@gmail.com](mailto:gaaapla7@gmail.com)**.

## Qué datos guarda y para qué

| Datos | Para qué |
|---|---|
| Tu correo | Crear tu cuenta y mandarte el código para entrar. |
| Nombre, edad, altura, peso, días disponibles y respuestas de salud del alta | Preparar un plan prudente y adaptado a ti. |
| Cómo estás cada día (sensaciones, molestias, sueño) | El semáforo que decide si hoy toca suave o descanso. |
| Salidas en bici (archivos FIT/GPX, recorrido, pulso, potencia) | Emparejarlas con el plan y enseñarte tu progreso. |
| Comida, peso, cintura y VO2 máx | Tus objetivos de comida y la tendencia del peso. |
| Datos del reloj (pasos, sueño, pulso en reposo) si lo conectas | Rellenar lo anterior sin que tengas que apuntarlo. |
| **Garmin Connect**, solo si lo conectas: tus actividades terminadas (fecha, tipo, tiempo, distancia, desnivel, pulso, potencia y cadencia, datos a lo largo de la salida y recorrido) y la clave que Garmin da a Bidea para recibirlas | Traer tus salidas a Bidea para tu plan, tu bici y tus zapatillas. Bidea solo **recibe** esos datos (nunca escribe en Garmin) y solo tú los ves. |
| **Strava**, solo si lo conectas: fecha, tipo, nombre, tiempo, distancia, desnivel, pulso, potencia y cadencia medios, datos a lo largo de la salida y recorrido de tus actividades; y, desde la 0.63, más datos de cada una: velocidad, potencia y pulso máximos, potencia ponderada, trabajo, calorías, temperatura, altura, dispositivo que la grabó, equipo (bici o zapatillas) que pusiste en Strava, la descripción que escribiste, vueltas, parciales por kilómetro, mejores esfuerzos y segmentos; y las claves que Strava da a Bidea para leerlas | Traer tus salidas a Bidea para tu plan, tu bici y tus zapatillas. Bidea solo **lee** (nunca escribe en Strava) y solo tú ves esos datos. |
| **Intervals.icu**, solo si lo vinculas: el permiso (token) que Intervals.icu da a Bidea al vincular tu cuenta y, de cada entreno planificado de tu plan, su fecha, tipo, nombre, descripción y duración | Poner tu plan de entrenos en tu calendario de Intervals.icu. Bidea solo **envía** entrenos: no lee tus actividades ni nada más de tu cuenta. El permiso solo deja escribir en tu calendario y se guarda **cifrado solo en tu móvil** (Keystore de Android), nunca en los servidores de Bidea ni en registros. |

| **Gimnasio**: las series que apuntas (ejercicio, fecha, repeticiones y kilos) | Enseñarte tu historial de cada ejercicio. Solo tú lo ves. |

Algunos son **datos de salud**. Solo se guardan porque das tu consentimiento al crear la cuenta, y puedes retirarlo en cualquier momento borrando la cuenta.

## Dónde se guardan

- En **Supabase**, en un servidor de la Unión Europea (Irlanda). Cada persona solo puede leer y escribir lo suyo.
- Algunas cosas se guardan en tu móvil y además se copian a tu cuenta (cambios de la rutina, casillas marcadas, comidas guardadas, tus bicis, tus zapatillas y los ajustes), para que no se pierdan al reinstalar o cambiar de móvil. El tipo y la foto de cada comida solo viven en tu móvil. Las fotos de comida se guardan reducidas y sin los datos del archivo original (como la ubicación), nunca se suben al servidor y se borran al quitar esa comida, al borrar tu cuenta o al desinstalar Bidea.
- **Gimnasio:** el catálogo de ejercicios (nombre, músculos, material y explicación) es el mismo para todo el mundo y no lleva datos tuyos. Tu rutina, lo que marcas como hecho y los PDF o fotos de rutinas que subes se quedan **solo en tu dispositivo** y se borran al borrar la cuenta o al entrar con otra. Las **fotos de los ejercicios** se cargan de GitHub (proyecto free-exercise-db): GitHub recibe tu dirección IP y qué fotos pides, nunca tu nombre ni tu correo.
- Los mapas de las salidas se cargan de Google Maps, y el buscador de alimentos consulta Open Food Facts. A Google le llega la zona del mapa que se ve (con tu recorrido dibujado encima en el propio móvil) y a Open Food Facts lo que buscas; nunca tu nombre, tu correo ni tus datos de salud. Google trata esos datos según su propia política de privacidad.

## La versión web para iPhone

En iPhone, Bidea se usa desde el navegador en [bidea.pages.dev/app](https://bidea.pages.dev/app/), con la misma cuenta y los mismos datos que en Android, guardados igual en Supabase (Unión Europea, Irlanda). La web está alojada en Cloudflare.

- Los archivos GPX o FIT que eliges se leen **en tu iPhone**; solo se sube el resumen de la salida (fecha, tipo, tiempo, distancia, desnivel, pulso y el recorrido).
- Para enseñarte el mapa, tu navegador pide los trozos de mapa a **OpenStreetMap** (servidores de la Fundación OpenStreetMap). Reciben tu dirección IP y qué trozos de mapa pides, es decir, la zona aproximada de la salida, pero no la forma del recorrido, que se dibuja en tu iPhone. No reciben tu nombre ni tu correo. En esta versión no se usa Google Maps. Si el mapa no carga, se dibuja el recorrido sin mapa.
- La web guarda en tu iPhone solo lo necesario para funcionar: tu sesión, el tema claro u oscuro, la copia de tus bicis y zapatillas, la hora del recordatorio y algunas preferencias sencillas. No usa cookies de publicidad ni de seguimiento.
- **Escáner de código de barras:** usa la cámara del iPhone solo mientras lo tienes abierto, para leer el código. La imagen se procesa en tu iPhone: no se guarda ni se envía a ningún sitio. A Open Food Facts solo le llega el número del código (o el texto que buscas) y tu dirección IP. El permiso de cámara lo concedes tú y puedes quitarlo en Ajustes del iPhone.
- **Recordatorio diario (opcional):** si lo activas, en Supabase se guardan la dirección del servicio de avisos de tu dispositivo (que Apple te asigna) con sus claves de cifrado, la hora que eliges y tu zona horaria. Solo sirven para mandarte un mensaje de ánimo a esa hora; el mensaje es el mismo para todo el mundo y no lleva datos tuyos. El aviso viaja por el servicio de notificaciones de Apple, que ve que Bidea te manda un aviso pero no su contenido de salud, porque no lleva ninguno. Se borra al apagarlo, al cerrar sesión o al borrar la cuenta, y te avisa solo si diste el permiso de notificaciones (puedes quitarlo en Ajustes del iPhone).
- **Foto de la comida (opcional):** puedes hacer una foto o elegirla de tu galería. Se reduce y se guarda **solo en tu iPhone** (en el almacenamiento del navegador), sin los datos del archivo original, como la ubicación. Nunca se sube al servidor y se borra al quitar esa comida, al cerrar sesión o al borrar la cuenta. Los permisos de cámara y fotos los concedes tú.
- **Gimnasio:** catálogo de ejercicios y tus series, como en Android. Tu rutina y lo que marcas como hecho se guardan solo en tu iPhone. Las fotos de los ejercicios se cargan de GitHub (free-exercise-db), que recibe tu dirección IP y qué fotos pides.
- **Revisión con Claude:** el PDF que te da Claude se lee **en tu iPhone**; no se sube. Se guarda su texto en el navegador de tu iPhone y se borra solo a las 2 semanas, al cerrar sesión o al borrar la cuenta.
- **Recordatorio:** Bidea te ofrece activarlo al entrar si está apagado, como mucho cada 3 días.
- Los conectores (Strava, Garmin, Health Connect) no existen en la versión web.

La política de la web (visitas, correos) está en [bidea.pages.dev/privacidad](https://bidea.pages.dev/privacidad).

## Lo que Bidea no hace

- No vende ni cede tus datos.
- No tiene anuncios ni rastreadores.
- No usa inteligencia artificial. La revisión con Claude la haces tú, desde tu propia cuenta de Claude, y solo con los datos que tú decides pegar. El PDF que te da Claude se lee en tu móvil, no se sube a ningún servidor y se borra solo a las 2 semanas.
- Familia: solo comparte tu resumen de salidas de 7 días con los correos que tú añadas, y nunca peso, comida ni salud. Las salidas que vienen de Strava no se incluyen.
- Strava: tus datos de Strava no se comparten con nadie, no se venden y no se usan para publicidad ni para entrenar modelos de inteligencia artificial. Puedes desconectarlo en Mi cuenta → Conectores: Bidea avisa a Strava, borra las salidas que vinieron de Strava y las claves guardadas. También puedes revocar el permiso desde tu cuenta de Strava. Borrar tu cuenta de Bidea elimina todo.
- Garmin Connect: los datos que llegan de Garmin se guardan en tu cuenta de Bidea, en Supabase (Unión Europea, Irlanda), que es el único tercero que los guarda o procesa, como proveedor de alojamiento. No se comparten con nadie más, no se venden, no se usan para publicidad y **nunca se usan para entrenar, evaluar ni mejorar modelos de inteligencia artificial**; Bidea no usa IA con ellos. Al desconectar Garmin, Bidea deja de recibirlos y borra las actividades que vinieron de Garmin y las claves guardadas; también puedes retirar el permiso desde tu cuenta de Garmin Connect. Puedes ver y exportar esos datos (Mi cuenta → Exportar a Excel) y borrarlos todos con **Borrar mi cuenta**.
- Intervals.icu: Bidea envía a Intervals.icu solo los entrenos planificados de tu plan, directamente desde tu móvil a tu cuenta, sin pasar por los servidores de Bidea. No se comparten con nadie más, no se venden, no se usan para publicidad ni para entrenar modelos de inteligencia artificial. Para desvincular: Mi cuenta → Conectores → Intervals.icu → Desvincular (borra el permiso del móvil); **Borrar mi cuenta** también lo borra. Los entrenos que ya estén en tu calendario de Intervals.icu quedan en tu cuenta de allí: bórralos desde Intervals.icu si quieres, y, si quieres, retira el permiso a Bidea desde los ajustes de tu cuenta de Intervals.icu. Su tratamiento allí lo rige la política de Intervals.icu.

## Tus derechos

- **Ver y llevarte tus datos:** Mi cuenta → Exportar a Excel.
- **Corregirlos:** desde la propia app, o escribiendo a gaaapla7@gmail.com.
- **Borrarlo todo:** Mi cuenta → **Borrar mi cuenta**. Se borran al momento tu cuenta y todos tus datos del servidor y del móvil (incluidos los de Strava y los de Garmin).
- Si crees que no se respetan tus derechos, puedes reclamar ante la Agencia Española de Protección de Datos (aepd.es).

## Edad

Bidea es solo para mayores de 18 años.

## Salud

Las recomendaciones de Bidea son generales y prudentes. No son consejo médico ni sustituyen a tu médico.
