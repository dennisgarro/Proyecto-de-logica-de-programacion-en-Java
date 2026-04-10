# LABORATORIO COMPLETO DE LÓGICA DE PROGRAMACIÓN

---

# 1. SECUENCIALES (Variables, Entrada y Salida)

---

## ¿Qué es un programa secuencial?

Un programa secuencial es aquel donde las instrucciones se ejecutan en orden, una después de otra, sin tomar decisiones ni repetir procesos.

Es decir, el flujo del programa sigue una línea directa desde el inicio hasta el final.

---

## ¿Qué es una variable?

Una variable es un espacio en memoria que se utiliza para almacenar información que puede cambiar durante la ejecución del programa.

---

## Tipos de datos más usados

* int: números enteros
* double: números decimales
* String: texto
* boolean: valores lógicos (verdadero o falso)

---

## ¿Por qué se utilizan?

Las variables permiten almacenar datos que el programa necesita para operar, procesar y mostrar resultados.

---

## Ejemplo

Leer el nombre y la edad de una persona y mostrarlos en pantalla.

---

## Explicación paso a paso

1. Se solicita información al usuario
2. Se almacenan los datos en variables
3. Se muestran los resultados en pantalla

---

## Algoritmo

```plaintext
INICIO
{
    edad es entero
    nombre es cadena

    muestre "Ingrese edad"
    lea edad

    muestre "Ingrese nombre"
    lea nombre

    muestre "Nombre: " + nombre
    muestre "Edad: " + edad
}
FIN
```

---

## Implementación en Java

```java
import java.util.Scanner;

public class Secuencial {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int edad;
        String nombre;

        System.out.println("Ingrese edad:");
        edad = sc.nextInt();

        System.out.println("Ingrese nombre:");
        nombre = sc.next();

        System.out.println("Nombre: " + nombre);
        System.out.println("Edad: " + edad);
    }
}
```

---

# 2. CONDICIONALES

---

## ¿Qué es una condicional?

Una estructura condicional permite tomar decisiones dentro de un programa, evaluando si una condición es verdadera o falsa.

---

## ¿Por qué se utilizan?

Se utilizan para ejecutar diferentes acciones dependiendo del resultado de una condición.

---

## Ejemplo

Determinar si una persona es mayor de edad.

---

## Explicación

El programa evalúa una condición:

* Si la edad es mayor o igual a 18, se considera mayor de edad
* En caso contrario, se considera menor de edad

---

## Algoritmo

```plaintext
INICIO
{
    edad es entero

    muestre "Ingrese edad"
    lea edad

    si edad >= 18 entonces
        muestre "Mayor de edad"
    si no
        muestre "Menor de edad"
}
FIN
```

---

## Implementación en Java

```java
import java.util.Scanner;

public class Condicional {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int edad;

        System.out.println("Ingrese edad:");
        edad = sc.nextInt();

        if (edad >= 18) {
            System.out.println("Mayor de edad");
        } else {
            System.out.println("Menor de edad");
        }
    }
}
```

---

# 3. CICLOS

---

## ¿Qué es un ciclo?

Un ciclo es una estructura que permite repetir un conjunto de instrucciones varias veces.

---

## ¿Por qué se utilizan?

Se utilizan para evitar repetir código manualmente y automatizar procesos repetitivos.

---

## Ejemplo

Mostrar los números del 1 al 5.

---

## Explicación

Se utiliza una variable de control que se incrementa en cada iteración hasta cumplir una condición.

---

## Algoritmo

```plaintext
INICIO
{
    para i desde 1 hasta 5
        muestre i
}
FIN
```

---

## Implementación en Java

```java
public class Ciclo {
    public static void main(String[] args) {

        for (int i = 1; i <= 5; i++) {
            System.out.println(i);
        }
    }
}
```

---

# 4. ARREGLOS

---

## ¿Qué es un arreglo?

Un arreglo es una estructura de datos que permite almacenar múltiples valores del mismo tipo en una sola variable.

---

## ¿Por qué se utilizan?

Permiten manejar varios datos de manera organizada y eficiente sin necesidad de crear múltiples variables.

---

## ¿Qué es un índice?

El índice es la posición de cada elemento dentro del arreglo.
Los índices comienzan desde 0.

---

## Ejemplo

Guardar 3 números y mostrarlos.

---

## Explicación

Se crea un arreglo con un tamaño definido.
Se utiliza un ciclo para ingresar los datos y otro para mostrarlos.

---

## Algoritmo

```plaintext
INICIO
{
    definir arreglo de tamaño 3

    para i desde 0 hasta 2
        lea numeros[i]

    para i desde 0 hasta 2
        muestre numeros[i]
}
FIN
```

---

## Implementación en Java

```java
import java.util.Scanner;

public class Arreglo {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int[] numeros = new int[3];

        for (int i = 0; i < 3; i++) {
            numeros[i] = sc.nextInt();
        }

        for (int i = 0; i < 3; i++) {
            System.out.println(numeros[i]);
        }
    }
}
```

---

# 5. MATRICES

---

## ¿Qué es una matriz?

Una matriz es un arreglo de dos dimensiones que organiza los datos en filas y columnas.

---

## ¿Por qué se utilizan?

Se utilizan para representar información estructurada como tablas.

---

## Ejemplo

Crear una matriz de 2x2 y mostrar sus valores.

---

## Explicación

Se utilizan dos ciclos anidados para recorrer filas y columnas.

---

## Algoritmo

```plaintext
INICIO
{
    matriz 2x2

    para i
        para j
            lea matriz[i][j]

    para i
        para j
            muestre matriz[i][j]
}
FIN
```

---

## Implementación en Java

```java
import java.util.Scanner;

public class Matriz {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int[][] matriz = new int[2][2];

        for (int i = 0; i < 2; i++) {
            for (int j = 0; j < 2; j++) {
                matriz[i][j] = sc.nextInt();
            }
        }

        for (int i = 0; i < 2; i++) {
            for (int j = 0; j < 2; j++) {
                System.out.print(matriz[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```

---

# 6. MATRICES DE OBJETOS

---

## ¿Qué es un objeto?

Un objeto es una representación de una entidad del mundo real que contiene atributos.

---

## ¿Qué es una matriz de objetos?

Es un arreglo donde cada posición contiene un objeto en lugar de un dato simple.

---

## Ejemplo

Almacenar estudiantes con nombre y nota.

---

## Explicación

Se define una clase, luego se crea un arreglo de objetos y se almacenan los datos.

---

## Algoritmo

```plaintext
INICIO
{
    definir Estudiante(nombre, nota)

    arreglo estudiantes[2]

    para i
        lea nombre y nota
        guardar estudiante

    para i
        muestre datos
}
FIN
```

---

## Implementación en Java

```java
class Estudiante {
    String nombre;
    double nota;
}

public class MatrizObjetos {
    public static void main(String[] args) {

        Estudiante[] estudiantes = new Estudiante[2];

        estudiantes[0] = new Estudiante();
        estudiantes[0].nombre = "Juan";
        estudiantes[0].nota = 4.5;

        estudiantes[1] = new Estudiante();
        estudiantes[1].nombre = "Ana";
        estudiantes[1].nota = 3.8;

        for (Estudiante e : estudiantes) {
            System.out.println(e.nombre + " - " + e.nota);
        }
    }
}
```

---

# CONCLUSIÓN

Este laboratorio permite desarrollar habilidades fundamentales en lógica de programación, desde el manejo básico de variables hasta estructuras más complejas como matrices y objetos.

El aprendizaje es progresivo, permitiendo al estudiante comprender paso a paso cómo resolver problemas mediante programación.
