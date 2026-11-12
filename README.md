<div align="center">

<img src="banner.png" width="820" alt="InnerTify"/>

</div>

InnerTify es un reproductor de música para Android que estoy haciendo yo, Diego Leo.
Aquí publico las APK y las notas de cada versión. El código lo llevo en un repositorio
privado.

[**Descargar la última versión**](https://github.com/DiegoLeo-commits/InnerTify-updates/releases/latest)

Ahora mismo la versión publicada es la **0.1.2**. La **1.1.1-Beta** todavía no está
subida; abajo te dejo lo que estoy cambiando.

## Instalar

1. Entra en el enlace de descarga y baja el `.apk`.
2. La primera vez Android te va a pedir permiso para instalar desde esa fuente.
3. Acepta e instala. Si ya tienes InnerTify, se actualiza encima sin borrar tus datos.

Necesitas Android 8.0 o superior y unos 60 MB libres.

## En la tele

El mismo APK sirve para el móvil y para Android TV / Google TV. No hay una versión
aparte: al instalarlo en la tele se abre su propio reproductor y aparece en el menú de
aplicaciones como InnerTify.

Para pasarlo a la tele puedes usar un pendrive, una app de enviar archivos, Downloader o
ADB:

```bash
adb connect <ip-de-la-tele>:5555
adb install InnerTify-<versión>-vc<code>.apk
```

Cuando la abras en la tele, deja la pantalla de espera visible. Desde el móvil entra en
**Conectar a un dispositivo** y elige la tele.

## Actualizaciones

La app revisa este repositorio y te avisa cuando hay una versión nueva. También puedes
comprobarlo a mano desde **Acerca de → versión**.

Si le das a «más tarde», esa versión no vuelve a molestar; la siguiente sí. Todas las APK
están firmadas con la misma clave, así que se instalan encima de la anterior.

## La 1.1.1-Beta, en preparación

Todavía no está publicada. Esto es lo que estoy terminando:

- **Canvas otra vez.** Spotify cambió la forma de pedir los videos y la app se quedó sin
  ellos un tiempo. Ya funciona de nuevo, con caché para que no tarden, y también se usa
  el video de YouTube cuando la canción no tiene Canvas de Spotify.
- **Modo inmersivo.** Con un Canvas de fondo, al tocar el reproductor quedan el video, la
  letra, la información de la canción y la barra de progreso. Sin los controles de
  reproducción encima. Si la canción no tiene Canvas, el toque no hace nada.
- **Letras.** Ya no cambian de tamaño ni mueven el resto de la pantalla según lo largas
  que sean. La línea entra con una animación más suave y las palabras se van iluminando
  de forma más natural. Al pasar de reproductor normal a inmersivo se sigue viendo la
  misma línea.
- **Repetir canción y temporizador.** El botón de repetir está abajo, junto a Compartir
  y Cola, y se pone verde cuando está activo. El temporizador también se pone verde y,
  si lo vuelves a tocar, te muestra cuánto queda.
- **Reproductor más parecido a Spotify.** Ajusté tamaños, espaciados y botones. Volvió el
  botón para transmitir a la tele y quité la X que duplicaba el gesto de cerrar.
- **Búsqueda.** Las búsquedas recientes ahora están en una pantalla aparte que se abre al
  tocar el campo. También dejé guardadas las portadas de las categorías, así que
  aparecen al instante y no vacías durante cinco segundos.
- **Cuenta e historial.** La cuenta quedó más simple, con la transferencia de playlists
  y Me gusta (experimental) como primera opción. Al historial le quité las estadísticas y
  lo dejé como una lista ordenada por días.
- **Detalles.** Banner nuevo, versión 1.1.1-Beta y pequeños ajustes en Acerca de.

## Archivos de cada versión

En cada release vas a encontrar el APK y un `latest.json` con la versión, el enlace, el
tamaño y el SHA-256. Ese archivo es el que consulta la app para saber si hay algo nuevo.

El nombre del APK lleva el `versionCode`; ese número es el que importa al actualizar. La
etiqueta del release es solo para leerlo.

## Comprobar una descarga

```bash
sha256sum InnerTify-<versión>-vc<code>.apk
```

El resultado tiene que coincidir con el `sha256` de `latest.json` y con el de las notas
del release.

## Aviso legal

InnerTify no está afiliado a Spotify. La música y las portadas son de sus respectivos
autores. Este repositorio no contiene código fuente ni concede derechos sobre él.

Hecho por **Diego Leo** · [TikTok](https://www.tiktok.com/@dieegoleo)
