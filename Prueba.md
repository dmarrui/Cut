**Herramienta "cut" en Linux:**

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

Supongamos que tienes un archivo de texto llamado `ejemplo.txt` con el siguiente contenido:

```plaintext
Juan,Perez,25
Maria,Gomez,30
Carlos,Ruiz,22
```

Este archivo representa información sobre personas, donde cada línea tiene el formato "Nombre,Apellido,Edad". Ahora, si deseas extraer solo los nombres (primer campo) de cada línea, puedes usar `cut` de la siguiente manera:

```bash
cut -d ',' -f 1 ejemplo.txt
```

Explicación de la línea de comando:

- `-d ','`: Especifica que el delimitador entre campos es la coma.
- `-f 1`: Indica que deseas extraer el primer campo.

La salida de este comando será:

Juan
Maria
Carlos

!![Mi Imagen]((https://github.com/dmarrui/Cut/images/2.png))

https://github.com/dmarrui/Cut/main/images/2.png

![Mi Imagen](imagenes/2.png)


Esto muestra únicamente la primera columna (nombres) de cada línea en el archivo.
