# Cómo trata Bidea tus datos

_Última actualización: 6 de noviembre de 2026 (versión 0.61 y versión web para iPhone)_

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
| **Strava**, solo si lo conectas: fecha, tipo, nombre, tiempo, distancia, desnivel, pulso, potencia y cadencia medios, datos a lo largo de la salida y recorrido de tus actividades; y las claves que Strava da a Bidea para leerlas | Traer tus salidas a Bidea para tu plan, tu bici y tus zapatillas. Bidea solo **lee** (nunca escribe en Strava) y solo tú ves esos datos. |

Algunos son **datos de salud**. Solo se guardan porque das tu consentimiento al crear la cuenta, y puedes retirarlo en cualquier momento borrando la cuenta.

## Dónde se guardan

- En **Supabase**, en un servidor de la Unión Europea (Irlanda). Cada persona solo puede leer y escribir lo suyo.
- Algunas cosas solo viven en tu móvil (cambios de la rutina, casillas marcadas, comidas guardadas, tu bici, y el tipo y la foto de cada comida). Las fotos de comida se guardan reducidas y sin los datos del archivo original (como la ubicación), nunca se suben al servidor y se borran al quitar esa comida, al borrar tu cuenta o al desinstalar Bidea.
- Los mapas de las salidas se cargan de Google Maps, y el buscador de alimentos consulta Open Food Facts. A Google le llega la zona del mapa que se ve (con tu recorrido dibujado encima en el propio móvil) y a Open Food Facts lo que buscas; nunca tu nombre, tu correo ni tus datos de salud. Google trata esos datos según su propia política de privacidad.

## La versión web para iPhone

En iPhone, Bidea se usa desde el navegador en [bidea.pages.dev/app](https://bidea.pages.dev/app/), con la misma cuenta y los mismos datos que en Android, guardados igual en Supabase (Unión Europea, Irlanda). La web está alojada en Cloudflare.

- Los archivos GPX o FIT que eliges se leen **en tu iPhone**; solo se sube el resumen de la salida (fecha, tipo, tiempo, distancia, desnivel, pulso y el recorrido).
- Para enseñarte el mapa, tu navegador pide los trozos de mapa a **OpenStreetMap** (servidores de la Fundación OpenStreetMap). Reciben tu dirección IP y qué trozos de mapa pides, es decir, la zona aproximada de la salida, pero no la forma del recorrido, que se dibuja en tu iPhone. No reciben tu nombre ni tu correo. En esta versión no se usa Google Maps. Si el mapa no carga, se dibuja el recorrido sin mapa.
- La web guarda en tu iPhone solo lo necesario para funcionar: tu sesión, el tema claro u oscuro y algunas preferencias sencillas. No usa cookies de publicidad ni de seguimiento.
- Conectores (Strava, Garmin, Health Connect), escáner de código de barras y fotos de comida no existen en la versión web.

La política de la web (visitas, correos) está en [bidea.pages.dev/privacidad](https://bidea.pages.dev/privacidad).

## Lo que Bidea no hace

- No vende ni cede tus datos.
- No tiene anuncios ni rastreadores.
- No usa inteligencia artificial. La revisión con Claude la haces tú, desde tu propia cuenta de Claude, y solo con los datos que tú decides pegar.
- Familia: solo comparte tu resumen de salidas de 7 días con los correos que tú añadas, y nunca peso, comida ni salud. Las salidas que vienen de Strava no se incluyen.
- Strava: tus datos de Strava no se comparten con nadie, no se venden y no se usan para publicidad ni para entrenar modelos de inteligencia artificial. Puedes desconectarlo en Mi cuenta → Conectores: Bidea avisa a Strava, borra las salidas que vinieron de Strava y las claves guardadas. También puedes revocar el permiso desde tu cuenta de Strava. Borrar tu cuenta de Bidea elimina todo.
- Garmin Connect: los datos que llegan de Garmin se guardan en tu cuenta de Bidea, en Supabase (Unión Europea, Irlanda), que es el único tercero que los guarda o procesa, como proveedor de alojamiento. No se comparten con nadie más, no se venden, no se usan para publicidad y **nunca se usan para entrenar, evaluar ni mejorar modelos de inteligencia artificial**; Bidea no usa IA con ellos. Al desconectar Garmin, Bidea deja de recibirlos y borra las actividades que vinieron de Garmin y las claves guardadas; también puedes retirar el permiso desde tu cuenta de Garmin Connect. Puedes ver y exportar esos datos (Mi cuenta → Exportar a Excel) y borrarlos todos con **Borrar mi cuenta**.

## Tus derechos

- **Ver y llevarte tus datos:** Mi cuenta → Exportar a Excel.
- **Corregirlos:** desde la propia app, o escribiendo a gaaapla7@gmail.com.
- **Borrarlo todo:** Mi cuenta → **Borrar mi cuenta**. Se borran al momento tu cuenta y todos tus datos del servidor y del móvil (incluidos los de Strava y los de Garmin).
- Si crees que no se respetan tus derechos, puedes reclamar ante la Agencia Española de Protección de Datos (aepd.es).

## Edad

Bidea es solo para mayores de 18 años.

## Salud

Las recomendaciones de Bidea son generales y prudentes. No son consejo médico ni sustituyen a tu médico.
