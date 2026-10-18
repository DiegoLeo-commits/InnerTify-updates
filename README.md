<div align="center">

<img src="logo.png" width="140" alt="InnerTify"/>

# InnerTify · Descargas

**Compilaciones oficiales de InnerTify.** Este repositorio solo contiene APKs y sus notas:
el código fuente vive en un repositorio privado.

[![Última versión](https://img.shields.io/github/v/release/DiegoLeo-commits/InnerTify-updates?style=flat-square&color=1DB954&label=versi%C3%B3n)](https://github.com/DiegoLeo-commits/InnerTify-updates/releases/latest)
[![Android](https://img.shields.io/badge/Android-8.0%2B-3DDC84?style=flat-square&logo=android&logoColor=white)](#instalar)
[![APK](https://img.shields.io/badge/tama%C3%B1o-~16%20MB-8A8A8A?style=flat-square)](#instalar)

[**Descargar la última versión →**](https://github.com/DiegoLeo-commits/InnerTify-updates/releases/latest)

</div>

---

## Instalar

1. Toca **Descargar la última versión** y abre el `.apk` desde la descarga.
2. Android pedirá permitir la instalación desde esa fuente la primera vez.
3. Acepta e instala. Si ya tienes InnerTify, se actualiza **encima** sin perder nada.

**Requisitos:** Android 8.0 o superior · ~60 MB libres.

## Actualizaciones

- Cada versión se publica aquí como un *release* con su APK y sus notas.
- La app consulta este repositorio sola y avisa cuando hay una versión nueva; también
  puedes revisar a mano desde **About → versión**.
- Si dices «más tarde», esa versión no vuelve a preguntar. La siguiente sí.
- Todas las compilaciones están firmadas con la misma clave, así que la actualización se
  instala encima de la anterior sin desinstalar.

## Qué hay en cada release

| Archivo | Para qué sirve |
| --- | --- |
| `InnerTify-<versión>-vc<code>.apk` | La app. Es el único archivo que necesitas. |
| `latest.json` | Metadatos que usa la app: versión, enlace, tamaño y SHA-256. |

El `versionCode` del nombre del APK es lo que compara la app; la etiqueta (`v0.1.0-preview`)
es solo para leerlo.

## Verificar una descarga

```bash
sha256sum InnerTify-0.1.0-Preview-vc19.apk
```

Debe coincidir con el `sha256` de `latest.json` y con el que aparece en las notas del release.

## Estado del proyecto

**0.1.0 Preview** — versión de prueba. Se irán agregando funciones en las próximas
actualizaciones; las novedades de cada una están en sus notas.

## Aviso legal

InnerTify no está afiliado a Spotify. Todo el contenido pertenece a sus creadores y se
ofrece tal cual. Spotify es una marca de Spotify AB. Este repositorio no contiene código
fuente ni concede ningún derecho sobre él (ver el repositorio privado del autor).

Hecho con 💚 por **Diego Leo** · [TikTok](https://www.tiktok.com/@dieegoleo)
