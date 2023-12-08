¡Buenas tardes! 

**Resumen de la herramienta "cut" en Linux:**

La herramienta "cut" en sistemas operativos basados en Unix y Linux se utiliza para extraer secciones específicas de líneas de texto de archivos o de la entrada estándar. Su función principal es recortar porciones de texto de cada línea y mostrar el resultado en la salida estándar.

**Sintaxis básica:**
```bash
cut [opciones] [archivo]
```

**Principales opciones:**
- **-c, --characters:** Especifica los caracteres a ser cortados.
- **-f, --fields:** Especifica los campos (columnas) a ser cortados.
- **-d, --delimiter:** Define el delimitador que separa los campos (por defecto es el carácter de tabulación).

**Ejemplos de uso:**
1. Cortar caracteres de una línea:
   ```bash
   cut -c 1-5 archivo.txt
   ```

2. Cortar campos de una línea delimitados por un carácter específico:
   ```bash
   cut -f 1,3 -d ',' archivo.csv
   ```

3. Cortar por delimitador de tabulación:
   ```bash
   cut -f 2 archivo.txt
   ```
