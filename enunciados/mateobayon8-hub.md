# Examen Parcial - mateobayon8-hub

**Usuario GitHub:** mateobayon8-hub
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 003

---

## Instrucciones

A continuación encontrarás 5 fragmentos de código extraídos de tus entregas. Cada fragmento contiene una o más situaciones relacionadas con los conceptos vistos en clase.

Para cada pregunta debes:
1) Identificar a qué se refiere la observación
2) Explicar si es o no un error y por qué
3) Proponer la corrección

Nota: Responde 5 de las 10 preguntas (elige libremente).


---

## Pregunta 1

Archivo: `Building.java` (Reto 003)

```java
for (int day = 0; day <= 6; day = day + 1) {
    for (int hour = 0; hour <= 23; hour = hour + 1) {
        // ...
    }
}
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `Building.java` (Reto 003)

```java
for (int height = 0; height <= 6; height = height + 1) {
    for (int width = 0; width <= 5; width = width + 1) {
        System.out.print(":");
        double chanceClosed = Math.random();
        double chanceLight = Math.random();
        int realHeight = 7 - height;
        if (width == 3) { System.out.print("[    ]:"); }
        // ... impresiones por ancho y etiqueta de planta
    }
}
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `Building.java` (Reto 003)

```java
if (chanceClosed < 0.70) {
    // ventanas cerradas
} else {
    if (chanceLight < 0.60) {
        // [*]
    } else {
        // [º]
    }
}
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `Building.java` (Reto 003)

```java
System.out.println(BASE_BUILDING1);
System.out.println(BASE_BUILDING2);
System.out.println(BASE_BUILDING3);
System.err.println("Day " + day + " " + hour + ":00 h");
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `Building.java` (Reto 003)

```java
final String separator = " _ __ ";
// ... se imprime al final de fila junto a Pn
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `changeCalculator.java` (Reto 001)

```java
public class changeCalculator {
    public static void main(String[] args) {
```

**¿Qué error hay en la declaración de la clase? Corrígelo.**

---

## Pregunta 7

Archivo: `WarriorVersusVampire.java` (Reto 002, líneas 17-24)

```java
System.out.println("[Narrator] You walk into a dark forest...");
System.out.println("(Press ENTER to continue)");
String enter1 = scanner.nextLine();
System.out.println("[Narrator] ... You feel a dark presence surround you...");
String enter2 = scanner.nextLine();
System.out.println("[Narrator] ... You hear steps coming towards you...");
String enter3 = scanner.nextLine();
System.out.println("[Narrator] ... It's Count Totemir! The most evil vampire in the country!");
String enter4 = scanner.nextLine();
```

**¿Qué error hay con las variables declaradas? Propón una solución.**

---

## Pregunta 8

Archivo: `Building.java` (Reto 003, líneas 6-13)

```java
final String ROOF_BUILDING1 = "               __/\\__              ";
final String ROOF_BUILDING2 = "  |    |    |  |####|  |    |    |  ";
final String ROOF_BUILDING3 = "====================================";

final String BASE_BUILDING1 = "     ==========================     ";
final String BASE_BUILDING2 = "   ==============================   ";
final String BASE_BUILDING3 = " ================================== ";

final String separator = " _ __ ";
```

**Analiza este código. ¿Qué errores encuentras?**

---

## Pregunta 9

Archivo: `Building.java` (Reto 003, línea 71)

```java
System.out.println(BASE_BUILDING3);

System.out.println();
System.err.println("Day " + day + " " + hour + ":00 h");
```

**¿Qué está mal en este código? Explica y corrige.**

---

## Pregunta 10

Archivo: `changeCalculator.java` (Reto 001, fragmento)

```java
int twoHundredBills = change > 200 ? change / 200 : 0;
change = change - (twoHundredBills * 200);

int oneHundredBills = change > 100 ? change / 100 : 0;
change = change - (oneHundredBills * 100);

int fiftyBills = change > 50 ? change / 50 : 0;
change = change - (fiftyBills * 50);
```

**Refactoriza este código:**

a) Elimina operadores innecesarios

b) Simplifica las operaciones

c) Muestra cómo quedaría una iteración mejorada

---

## Criterios de evaluación

- Identificación correcta del error: 40%
- Explicación del porqué es un error: 30%
- Propuesta de corrección válida: 30%

