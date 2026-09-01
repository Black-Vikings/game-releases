# Black Vikings — builds publicados

Acá viven las versiones jugables de nuestros juegos. Una carpeta por juego.

## Cómo se descarga

**Los binarios no están en el árbol de archivos: están en los
[releases](../../releases).** Un build pesa unos 60 MB y tres sistemas por
versión son casi 200; metidos en el repositorio, cada persona que lo clona se
llevaría todas las versiones que existieron alguna vez, para siempre.

Buscá tu juego y tu sistema:

| Archivo | Para |
|---|---|
| `<juego>-<version>-windows.zip` | Windows 10 y 11, 64 bits |
| `<juego>-<version>-linux.zip` | Linux 64 bits |
| `<juego>-<version>-macos.zip` | macOS, Intel y Apple Silicon |

En Windows, descomprimí la carpeta entera antes de ejecutar. El `.exe` suelto no
encuentra sus datos.

En macOS, la primera vez hay que abrirlo con clic derecho → Abrir: no está
firmado con una cuenta de desarrollador de Apple, así que el doble clic lo
bloquea sin explicar por qué.

## Qué hay en cada carpeta

Lo que **no** es un binario: las notas de cada versión, qué cambió y qué se
sabe que está roto. Eso sí conviene poder leerlo sin descargar nada.

```
robadados/
  README.md          quién es, cómo se juega, requisitos
  v0.1.0/NOTAS.md    qué trae, qué falta, qué está roto
```

## De dónde salen

De un pipeline en el repositorio privado de cada juego. Nadie sube un build a
mano: se etiqueta una versión, y el pipeline exporta los tres sistemas desde el
mismo commit y publica el release acá.

Que salgan los tres del mismo commit no es burocracia. Un build de Windows de
ayer y uno de Linux de hoy son dos juegos distintos, y descubrirlo cuando dos
amigos no pueden jugar juntos es tarde.
