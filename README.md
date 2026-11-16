# Sistema de Ventas e Inventario - Glamour Makeup Sinaloa (Unidad 3)

- **Materia:** Lenguajes de Interfaz | **Docente:** Dr. Jose Luis Medina Jimenez
- **Alumnas:** Natalia Lopez Ibarra, Frida Sofia Vega Vazquez

Programa de consola en ensamblador x86 de 32 bits (MASM) con Irvine32. Version de la Unidad 3: macros (`mImprimir`, `mLeerCadena`, `mCopiarBloque`, `mIrAlFinCadena`, `mGuardarArchivo`), operador `USES` y procedimientos reutilizables. Regla adicional: 10% de descuento en ventas de 3 o mas unidades.

## Estructura del repositorio
| Ruta | Contenido |
|---|---|
| `ProyectoVS/` | Proyecto de Visual Studio: `main.asm` |
| `catalogo.dat` | Inventario de prueba (binario, 440 bytes, 4 productos) |
| `catalogo.txt` | El mismo inventario en texto legible (solo para consultar) |
| `main_U2.asm` | Version de la Unidad 2 (para la comparacion antes/despues) |
| `Informe.md` | Reporte con la seccion "Version de la Unidad 3" |

## Compilacion (Visual Studio 2022 + plantilla Irvine32 de la clase)
1. Abre el proyecto Irvine32 que usas en clase (el que ya compila tus practicas).
2. Reemplaza su `.asm` por `ProyectoVS/main.asm` (o agregalo y quita el anterior).
3. Plataforma **x86 (Win32)**, configuracion Debug.
4. Compila (Ctrl+Shift+B) y ejecuta (Ctrl+F5).

## Inventario de prueba
Copia `catalogo.dat` a la **carpeta de trabajo** del proyecto (la que contiene el `.vcxproj`; si ejecutas el `.exe` directamente, junto al `.exe`). Al iniciar, el programa carga `catalogo.dat`; si no existe, arranca vacio.

El programa genera solos: `catalogo.dat`, `catalogo.txt`, `movimientos.txt` y `ventas.txt` (se guardan despues de cada alta, entrada y venta). `catalogo.dat` es binario; para leerlo usa `catalogo.txt`.

## Menu
1. Registrar producto  2. Consultar inventario  3. Recibir mercancia  4. Vender producto  5. Mostrar resumen  6. Salir

## Pruebas
Tabla completa en `Informe.md`, seccion 7.4.
