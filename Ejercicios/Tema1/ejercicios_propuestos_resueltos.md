# Ejercicios Resueltos `PROG03_Ejercicios`

### Ejercicios Resueltos con Explicaciones

#### Ejercicio 1
**Escribe un programa que dé los "buenos días".**

**Descripción:**
El objetivo de este ejercicio es crear un programa básico que imprima un mensaje simple en pantalla utilizando la función `System.out.println`.

```java
public class BuenosDias {
    public static void main(String[] args) {
        System.out.println("Buenos días");
    }
}
```

#### Ejercicio 2
**Escribe un programa que calcule y muestre el área de un cuadrado de lado igual a 5.**

**Descripción:**
El área de un cuadrado se calcula con la fórmula `lado * lado`. Este programa utiliza una variable fija para representar el lado del cuadrado.

```java
public class AreaCuadrado {
    public static void main(String[] args) {
        int lado = 5; // Lado del cuadrado
        int area = lado * lado; // Cálculo del área
        System.out.println("El área del cuadrado es: " + area);
    }
}
```

#### Ejercicio 3
**Escribe un programa que calcule el área de un cuadrado cuyo lado se introduce por teclado.**

**Descripción:**
En este ejercicio se pide al usuario que introduzca el valor del lado mediante el teclado. Utilizamos la clase `Scanner` para recibir la entrada.

```java
import java.util.Scanner;

public class AreaCuadradoInput {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el lado del cuadrado: ");
        int lado = scanner.nextInt(); // Lectura del lado
        int area = lado * lado; // Cálculo del área
        System.out.println("El área del cuadrado es: " + area);
    }
}
```

#### Ejercicio 4
**Escribe un programa que lea dos números, calcule y muestre el valor de su suma, resta, producto y división.**

**Descripción:**
El programa solicita dos números al usuario, realiza operaciones básicas y muestra los resultados. Consideramos el caso especial de la división por cero.

```java
import java.util.Scanner;

public class OperacionesBasicas {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el primer número: ");
        double num1 = scanner.nextDouble();
        System.out.print("Introduce el segundo número: ");
        double num2 = scanner.nextDouble();

        // Realizamos y mostramos las operaciones
        System.out.println("Suma: " + (num1 + num2));
        System.out.println("Resta: " + (num1 - num2));
        System.out.println("Producto: " + (num1 * num2));
        if (num2 != 0) {
            System.out.println("División: " + (num1 / num2));
        } else {
            System.out.println("Error: División por cero.");
        }
    }
}
```

#### Ejercicio 5
**Escribe un programa que toma como dato de entrada un número que corresponde a la longitud de un radio y nos escribe la longitud de la circunferencia, el área del círculo y el volumen de la esfera que corresponden con dicho radio.**

**Descripción:**
Este ejercicio utiliza fórmulas matemáticas para calcular:
- Longitud de la circunferencia: `2 * π * radio`
- Área del círculo: `π * radio²`
- Volumen de la esfera: `(4/3) * π * radio³`

Usamos la clase `Math` para operaciones matemáticas.

```java
import java.util.Scanner;

public class Geometria {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el radio: ");
        double radio = scanner.nextDouble(); // Lectura del radio

        // Cálculos matemáticos
        double longitud = 2 * Math.PI * radio;
        double area = Math.PI * Math.pow(radio, 2);
        double volumen = (4.0 / 3) * Math.PI * Math.pow(radio, 3);

        // Mostrar resultados
        System.out.println("Longitud de la circunferencia: " + longitud);
        System.out.println("Área del círculo: " + area);
        System.out.println("Volumen de la esfera: " + volumen);
    }
}
```

#### Ejercicio 6
**Escribe un programa que dado el precio de un artículo y el precio de venta real nos muestre el porcentaje de descuento realizado.**

**Descripción:**
El programa calcula el porcentaje de descuento con la fórmula:
`descuento = ((precioOriginal - precioVenta) / precioOriginal) * 100`

```java
import java.util.Scanner;

public class Descuento {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Introduce el precio original: ");
        double precioOriginal = scanner.nextDouble();
        System.out.print("Introduce el precio de venta: ");
        double precioVenta = scanner.nextDouble();

        // Cálculo del descuento
        double descuento = ((precioOriginal - precioVenta) / precioOriginal) * 100;
        System.out.println("El porcentaje de descuento es: " + descuento + "%");
    }
}
```

---

Si necesitas más ejercicios resueltos, házmelo saber.

