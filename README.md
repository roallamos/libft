# Libft

## Descripción

Libft es un proyecto del curso de la Escuela 42 que consiste en crear tu propia biblioteca de funciones en C. Esta biblioteca puede contener funciones que se utilizan comúnmente en proyectos futuros, así como funciones personalizadas que te ayuden a abordar desafíos específicos de programación.

## Características

- Implementación de una biblioteca de funciones en C.
- Funciones estándar de la biblioteca C (`libc`) y funciones personalizadas.

## Requisitos

- Sistema operativo: Linux.
- Compilador compatible con C.

## Instalación

1. Clona este repositorio:
    ```sh
    git clone https://github.com/roallamos/libft.git
    ```
2. Navega al directorio del proyecto:
    ```sh
    cd libft
    ```
3. Compila la biblioteca:
    ```sh
    make
    ```

## Uso

1. Para utilizar la biblioteca en tus proyectos, incluye el archivo `libft.h` en tus archivos de código fuente.
    ```c
    #include "libft.h"
    ```

2. Compila tu proyecto con la biblioteca `libft.a` utilizando el siguiente comando:
    ```sh
    gcc -o mi_programa mi_programa.c -L. -lft
    ```

## Contenido

La biblioteca Libft contiene una amplia gama de funciones divididas en varias categorías, que incluyen:

- Funciones de manejo de memoria (`calloc`, `memset`, `memcpy`, etc.).
- Funciones de manejo de cadenas (`strlen`, `strcpy`, `strcat`, etc.).
- Funciones de manejo de caracteres (`isdigit`, `isalpha`, `tolower`, etc.).
- Funciones de lista enlazada (`lstnew`, `lstadd_back`, `lstsize`, etc.).
- Y muchas más.

Para obtener una lista completa de las funciones disponibles, consulta el archivo `libft.h`.

## Ejemplo de Uso

```c
#include "libft.h"

int main(void)
{
    char *str = "Hello, world!";
    int len = ft_strlen(str);
    ft_putstr("Length of string: ");
    ft_putnbr(len);
    ft_putchar('\n');
    return (0);
}
