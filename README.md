# Lordstream [(Dockerfile)](https://github.com/Lordpedal/Lordstream)

Basado en **ACEstream** es un sencillo **reproductor de streaming**, compatible con los principales reproductores de video.

## Dockerfile

La imagen esta creada sobre Ubuntu 20.04. Solo incluye soporte arquitecturas **AMD64**

## Uso

Compatible con los esquemas docker-compose v2.

```
version: "2"
services:
  iptv:
    image: lordpedal/lordstream
    container_name: LordStream
    environment:
      - TZ=Europe/Madrid
    network_mode: host
    restart: always
```

## Parámetros

Las imágenes de contenedor se configuran utilizando parámetros pasados en tiempo de ejecución (como los anteriores). 
Estos parámetros están separados por dos puntos e indican ``<external>: <internal>`` respectivamente. 

| Parámetro | Función |
| ------ | ------ |
| ``TZ=Europe/Madrid`` | Zona horaria |
| ``Modo Red: host`` | Habilitamos el uso de la red ``host`` en vez de una virtual para docker |

## Gestión Web

Interfaces web

http://localhost:8000/stat

http://localhost:6878/webui/app/password/server

## [Overclock Server](https://lordpedal.github.io)

#### ... la culminación de un fin es el comienzo de una realidad.
