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
# SECUENCIALES (25 ejercicios)
1.	Leer un número y mostrarlo
2.	Leer dos números y mostrar su suma
3.	Leer tres números y mostrar el promedio
4.	Leer el nombre de una persona y mostrar un saludo
5.	Leer edad y mostrarla
6.	Leer base y altura y calcular área de un triángulo
7.	Leer radio y calcular área de un círculo
8.	Leer un número y mostrar su doble
9.	Leer un número y mostrar su triple
10.	Leer dos números y mostrar resta y multiplicación
11.	Leer horas trabajadas y valor hora, calcular salario
12.	Leer temperatura en Celsius y convertir a Fahrenheit
13.	Leer distancia y tiempo, calcular velocidad
14.	Leer precio y cantidad, calcular total
15.	Leer nombre, edad y ciudad y mostrarlos
16.	Leer 4 números y mostrar el mayor
17.	Leer un número y calcular su cuadrado
18.	Leer un número y calcular su cubo
19.	Leer largo y ancho de un rectángulo y calcular área
20.	Leer 5 números y mostrar su suma
21.	Leer un número y mostrar su raíz cuadrada
22.	Leer capital y tasa, calcular interés simple
23.	Leer un número y mostrar la mitad
24.	Leer nombre completo y mostrarlo
25.	Leer dos números y mostrar el mayor

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
# CONDICIONALES (25 ejercicios)
1.	Determinar si un número es positivo o negativo
2.	Determinar si un número es par o impar
3.	Validar si una persona es mayor de edad
4.	Leer dos números y mostrar el mayor
5.	Determinar si un número es múltiplo de 5
6.	Leer tres números y mostrar el mayor
7.	Validar si un estudiante aprueba (nota ≥ 3)
8.	Determinar si un número está entre 10 y 20
9.	Leer edad y clasificar (niño, joven, adulto)
10.	Validar si un número es divisible entre 3 y 5
11.	Leer salario y aplicar aumento si es menor a cierto valor
12.	Validar si una letra es vocal
13.	Determinar si un año es bisiesto
14.	Leer tres números y ordenarlos
15.	Validar si un número es primo
16.	Leer temperatura y clasificar clima
17.	Determinar si un número es mayor que 100
18.	Validar usuario y contraseña
19.	Leer dos números y mostrar el menor
20.	Determinar si puede votar
21.	Clasificar nota (bajo, medio, alto)
22.	Validar si un número está en un rango
23.	Determinar tipo de triángulo
24.	Validar si un número es negativo, cero o positivo
25.	Determinar si una persona puede entrar a un evento

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
# CICLOS (25 ejercicios)
1.	Mostrar números del 1 al 10
2.	Mostrar números del 10 al 1
3.	Mostrar números pares del 1 al 20
4.	Mostrar números impares del 1 al 20
5.	Sumar números del 1 al 10
6.	Mostrar tabla de multiplicar de un número
7.	Contar cuántos números ingresa el usuario
8.	Sumar números hasta que el usuario ingrese 0
9.	Mostrar múltiplos de 3
10.	Calcular factorial de un número
11.	Mostrar los primeros n números
12.	Contar números positivos ingresados
13.	Contar números negativos
14.	Mostrar suma de números pares
15.	Mostrar promedio de números ingresados
16.	Validar contraseña hasta que sea correcta
17.	Mostrar tabla del 1 al 10
18.	Leer 10 números y mostrarlos
19.	Determinar mayor de varios números
20.	Contar números mayores a 50
21.	Mostrar serie Fibonacci
22.	Sumar números impares
23.	Contar cuántos son pares
24.	Mostrar números hasta cierto límite
25.	Generar patrón de asteriscos

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
# ARREGLOS (25 ejercicios)
1.	Guardar 5 números y mostrarlos
2.	Calcular suma de un arreglo
3.	Calcular promedio de un arreglo
4.	Mostrar el mayor valor
5.	Mostrar el menor valor
6.	Contar números pares
7.	Contar números impares
8.	Buscar un número
9.	Ordenar arreglo ascendente
10.	Ordenar arreglo descendente
11.	Invertir arreglo
12.	Copiar arreglo a otro
13.	Sumar dos arreglos
14.	Mostrar posiciones de un valor
15.	Contar repetidos
16.	Eliminar un elemento
17.	Insertar un elemento
18.	Comparar dos arreglos
19.	Buscar el segundo mayor
20.	Contar mayores a un valor
21.	Reemplazar valores
22.	Mostrar solo pares
23.	Mostrar solo impares
24.	Rotar arreglo
25.	Validar si está ordenado

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
#  MATRICES (25 ejercicios)
1.	Crear matriz 2x2 y mostrarla
2.	Sumar todos los elementos
3.	Mostrar diagonal principal
4.	Mostrar diagonal secundaria
5.	Sumar filas
6.	Sumar columnas
7.	Encontrar mayor
8.	Encontrar menor
9.	Contar pares
10.	Contar impares
11.	Transponer matriz
12.	Multiplicar matrices
13.	Sumar matrices
14.	Buscar elemento
15.	Contar repetidos
16.	Ordenar matriz
17.	Mostrar bordes
18.	Promedio de matriz
19.	Validar matriz identidad
20.	Validar matriz simétrica
21.	Invertir matriz
22.	Rotar matriz
23.	Contar mayores a valor
24.	Mostrar filas pares
25.	Mostrar columnas impares

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
# MATRICES DE OBJETOS (25 ejercicios)
1.	Guardar estudiantes y mostrarlos
2.	Calcular promedio de notas
3.	Mostrar estudiante con mayor nota
4.	Mostrar estudiante con menor nota
5.	Buscar estudiante por nombre
6.	Contar aprobados
7.	Contar reprobados
8.	Ordenar por nota
9.	Ordenar por nombre
10.	Mostrar lista invertida
11.	Filtrar por nota
12.	Actualizar datos
13.	Eliminar estudiante
14.	Insertar estudiante
15.	Promedio general
16.	Mostrar estudiantes destacados
17.	Validar si existe estudiante
18.	Contar por rango de notas
19.	Agrupar estudiantes
20.	Mostrar top 3
21.	Buscar coincidencias
22.	Calcular estadísticas
23.	Filtrar por condición
24.	Mostrar estudiantes en orden
25.	Simular sistema académico básico

---

# CONCLUSIÓN

Este laboratorio permite desarrollar habilidades fundamentales en lógica de programación, desde el manejo básico de variables hasta estructuras más complejas como matrices y objetos.

El aprendizaje es progresivo, permitiendo al estudiante comprender paso a paso cómo resolver problemas mediante programación.
