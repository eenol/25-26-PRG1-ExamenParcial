# Examen Parcial - eenol

**Usuario GitHub:** eenol
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 003

---

## Instrucciones

A continuación encontrarás fragmentos de código extraídos de tus entregas. Cada fragmento contiene una o más situaciones relacionadas con los conceptos vistos en clase.

Para cada pregunta debes:
1) Identificar a qué se refiere la observación
2) Explicar si es o no un error y por qué
3) Proponer la corrección

Nota: Responde 5 de las 10 preguntas (en función a lo indicado en el examen).


---

## Pregunta 1

Archivo: `SimulacionHotel.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/61896085e1000d61811ce32fcf7eb625aa69f23f/entregas/hidalgoenol/SimulacionHotel.java) (Reto 003)

```java
class SimulacionHotel {
    public static void main(String[] args) {
        // ...
    }
}
```

¿Qué observas en este código?


En este código se puede apreciar como falta poner un public delante del "class SimulacionHotel" debido a que en Java hay una regla la cual dice que si el archivo tiene una clase con su mismo nombre esta debe ser pública, además el nombre de estas deben coincidir a la perfección y tan solo puede haber una por cada programa. No definir esto como public nos podría llevar a un error a la hora de ejecutar o puede ser que no compile; por tanto la manera de arreglar esto sería modificádolo la linea número cinco por: "public class SimulacionHotel {".
---

## Pregunta 2

Archivo: `SimulacionHotel.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/61896085e1000d61811ce32fcf7eb625aa69f23f/entregas/hidalgoenol/SimulacionHotel.java) (Reto 003)

```java
while (dia <= DIAS) {
    int consumoDia = 0;
    // ...
    int hora = 0;
    while (hora < HORAS) {
        // ...
        hora++;
    }
}
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `SimulacionHotel.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/61896085e1000d61811ce32fcf7eb625aa69f23f/entregas/hidalgoenol/SimulacionHotel.java) (Reto 003)

```java
if (hayRayo && c == columnaRayo) {
    celda = "[X]";
} else if (hayMantenimiento && p == plantaMantenimiento && hora >= horaMantenimiento) {
    celda = "[#]";
} else if (persianaAbierta && luzEncendida) {
    celda = "[*]";
    consumoDia++;
} else if (persianaAbierta && !luzEncendida) {
    celda = "[º]";
} else {
    celda = "[ ]";
}
```

¿Qué observas en este código?


Este creo que es el error mas grande ya que también se trata de programación, el “rayo” ([X]) y el “mantenimiento” ([#]) pueden como colapsar entre ellos. Ya que si en una planta hay mantenimiento y en esa misma columna cae un rayo, solo se ejecutará la primera condición ([X]), y el mantenimiento no se hará. La solución es crear un nuevo programa que pueda abarcar ambos. Además, se usa "hora >= horaMantenimiento", que quiere decir que cuando pase la hora de mantenimiento, la planta quedará en mantenimiento hasta el final del día, habria que utilizar "==". Yo lo arreglaría de la siguiente forma:
if (hayRayo && c == columnaRayo) {
    celda = "[X]";  // El rayo tiene prioridad máxima
} else if (hayMantenimiento && p == plantaMantenimiento && hora == horaMantenimiento) {
    celda = "[#]";  // Solo ocurre en esa hora concreta
} else if (persianaAbierta && luzEncendida) {
    celda = "[*]";
    consumoDia++;
} else if (persianaAbierta) {
    celda = "[º]";
} else {
    celda = "[ ]";
}

---

## Pregunta 4

Archivo: `SimulacionHotel.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/61896085e1000d61811ce32fcf7eb625aa69f23f/entregas/hidalgoenol/SimulacionHotel.java) (Reto 003)

```java
System.out.println("Dia " + dia + " - " + hora + ":00  Consumo hora: " + consumoDia);
```

¿Qué observas en este código?


En este código observo como la estructura es correcta, usamos "System.out.println()" para imprimir un texto por pantalla y dentro de este casi todo esta bien; en esta linea del programa lo que tratamos de hacer es que una vez finalizado haga una recogida de datos, el problema de mi linea de código es que a la hora de decir el consumo por hora, se esta diciendo el consumo diario ya que habría que sustituir "consumoDia" por "consumoHora" una variable la cual habría que crear; es un error lógico y que no da error en el código pero no estaría siendo un programa realista, sería confuso.
---

## Pregunta 5

Archivo: `SimulacionHotel.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/61896085e1000d61811ce32fcf7eb625aa69f23f/entregas/hidalgoenol/SimulacionHotel.java) (Reto 003)

```java
System.out.println("Media semanal: " + (consumoTotalSemana / 7));
```

¿Qué observas en este código?


En esta parte del código hay un problea grave, estamos dividiendo un entero entre otro(Int), el problema es que esta división va a realizar un redondeo hacia abajo, por lo que nuestro resultado no estaría siendo nada realista; la solución a esta linea del código es añadir un double para que así de esta forma nos pueda dar un número decimal y pueda ser mucho mas exacto, esta linea de código arreglada quedaría así: "System.out.println("Media semanal: " + ((double) consumoTotalSemana / 7));" de esta forma ya da igual que la division sea exacta o no, si no lo es habrá decimales.

---

## Pregunta 6

Archivo: `Edificio.java` — [PRs del alumno](https://github.com/mmasias/25-26-PRG1/pulls?q=is%3Apr+author%3Aeenol+is%3Aall) (Reto 003, línea 3)

```java
final String TECHO_DEL_EDIFICIO = "               __/\\__";
final String PARTE_DEABJO_DEL_TECHO = "  |    |    |  |####|  |    |    |  ";
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `Edificio.java` — [PRs del alumno](https://github.com/mmasias/25-26-PRG1/pulls?q=is%3Apr+author%3Aeenol+is%3Aall) (Reto 003, línea 18)

```java
boolean luzEncencida, persianaAbierta;
```

¿Qué observas en este código?


En este código se observa como hay variables que no estan bien nombradas, en Java, los nombres de las variables deben coincidir exactamente, si en otra parte del código usamos "luzEncendida", el compilador mostrará un error como este: "cannot find symbol: variable luzEncendida", por lo que este código se solucionaría sustituyendo: "boolean luzEncencida, persianaAbierta;" por :"boolean luzEncendida, persianaAbierta;"
---

## Pregunta 8

Archivo: `Edificio.java` — [PRs del alumno](https://github.com/mmasias/25-26-PRG1/pulls?q=is%3Apr+author%3Aeenol+is%3Aall) (Reto 003, líneas 26-34)

```java
for (int planta = 1; planta <= PLANTA_MAXIMA; planta++) {
    for (int columna = 1; columna <= 6; columna++) {
        persianaAbierta = Math.random() < PROBABILIDAD_PERSIANA_ABIERTA;
        luzEncencida = Math.random() < PROBABILIDAD_LUZ_ENCENDIDA;

        System.out.print(
                !persianaAbierta ? VENTANA_CERRADA
                        : luzEncencida ? VENTANA_LUZ_ENCENDIDA : VENTANA_LUZ_APAGADA);
```

¿Qué observas en este código?

---

## Pregunta 9

Archivo: `Edificio.java` — [PRs del alumno](https://github.com/mmasias/25-26-PRG1/pulls?q=is%3Apr+author%3Aeenol+is%3Aall) (Reto 003, línea 37)

```java
System.out.print("- P" + (PLANTA_MAXIMA + 1 - planta));
```

¿Qué observas en este código?

---

## Pregunta 10

Archivo: `Edificio.java` — [PRs del alumno](https://github.com/mmasias/25-26-PRG1/pulls?q=is%3Apr+author%3Aeenol+is%3Aall) (Reto 003, línea 1)

```java
public class Edificio {
```

¿Qué observas en este código?

