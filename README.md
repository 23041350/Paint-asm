# PaintOk.asm – Paint básico para DOS en modo VGA 13h

**PaintOk** es un programa tipo “Paint” desarrollado en lenguaje ensamblador (sintaxis Intel, TASM) que funciona en modo real de DOS. Utiliza el modo gráfico VGA 13h (320×200 píxeles, 256 colores) y permite dibujar con el mouse, seleccionar colores desde una paleta o con teclas numéricas, ajustar el tamaño del pincel, limpiar la pantalla y salir con ESC.

> Este proyecto fue realizado para la asignatura *Lenguajes de Interfaz* de Ingeniería en Sistemas Computacionales.

## Capturas de pantalla

*(Aquí puedes añadir imágenes del programa en ejecución dentro de DOSBox)*

## Requisitos

- **DOSBox** (emulador) – [Descargar DOSBox](https://www.dosbox.com)
- **GUI Turbo Assembler** (IDE con TASM/TLINK) o bien TASM y TLINK por separado.
- Sistema operativo: Windows, Linux o macOS (con DOSBox y las herramientas de ensamblado en emulación o nativas).

## Compilación y generación del ejecutable

El archivo fuente es `PaintOk.asm`. Para obtener `PaintOk.exe` sigue estos pasos:

### Opción A: Usando GUI Turbo Assembler (Windows)

1. Instala [GUI Turbo Assembler](https://sourceforge.net/projects/guiturboassembler/).
2. Abre el IDE, carga `PaintOk.asm`.
3. Presiona `Alt + A, Alt + B` (Compile) para ensamblar y enlazar automáticamente.
4. El ejecutable `PaintOk.exe` se generará en la misma carpeta.

### Opción B: Línea de comandos (TASM/TLINK)

```bash
tasm PaintOk.asm
tlink PaintOk.obj
