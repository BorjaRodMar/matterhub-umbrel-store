# Matter Hub — Umbrel Community App Store

Tienda de comunidad para Umbrel que instala
[home-assistant-matter-hub (HAMH)](https://github.com/riddix/home-assistant-matter-hub),
un bridge Matter que expone entidades de Home Assistant a controladores como
Alexa, Google Home o Apple Home mediante comunicación local.

## Instalación

1. En Umbrel: **App Store → ⋮ → Community App Stores**.
2. Añade la URL de este repositorio y pulsa **Add**.
3. Instala **Matter Hub** desde la tienda.

## Configuración

La app necesita un token de acceso de larga duración de Home Assistant.
Por seguridad, el token **no** se incluye en este repositorio: se inyecta
localmente en el archivo de entorno de la app en el propio Umbrel.

La interfaz de gestión queda disponible en el puerto **8482** del host.

## Requisitos

- Home Assistant accesible en la red local.
- `network_mode: host` (necesario para Matter / mDNS).
- IPv6 operativo en la red.

## Contenido del repositorio

- `umbrel-app-store.yml` — manifiesto de la tienda.
- `matter-hub/umbrel-app.yml` — manifiesto de la app.
- `matter-hub/docker-compose.yml` — definición del contenedor.

## Nota

Tienda de uso personal. HAMH es un proyecto de
[RiDDiX](https://github.com/riddix/home-assistant-matter-hub);
este repositorio solo lo empaqueta para Umbrel.
