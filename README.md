Junto al script del peyecto está subida 1 carpeta llena de subcarpetas y de archivos .txt.
Solo tienen texto aleatorio, excepto algunos q tienen N° de serie a buscar

Este es un programa que se encargua de buscar números de serie que cumplan un determinado formato, dentro de un arbol de carpetas.
Va a buscar cualquier string que coincida con un patrón de número de serie. Sabemos que no puede haber más de un número de serie por archivo.

Se usó el módulo os con el método walk() para iterear el directorio, y las expresiones regulares para encontrar el formato de número de serie
Se usó modulo time para medir el tiempo q lleva la ejec del script

A los fines de este ejercicio, estas son las condiciones de formato que deben cumplir los hallazgos:
- [N] + [tres carateres de texto] + [-] + [5 números]

patron = r'N\D{3}-\d{5}'

Por ejemplo: Nryu-12365

La presentación en pantalla de los hallazgos es un listado en formato de tabla, que tiene el siguiente formato de ejemplo:

----------------------------------------------------
Fecha de búsqueda: [fecha de hoy]

ARCHIVO		NRO. SERIE
-------		----------
texto1.txt	Nter-15496
texto25.txt	Ngba-85235

Números encontrados: 2
Duración de la búsqueda: 1 segundos

----------------------------------------------------
