# Examen Parcial - izanherranz07

**Usuario GitHub:** izanherranz07
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 003

---

## Instrucciones

A continuación encontrarás 5 fragmentos de código extraídos de tus entregas. Cada fragmento contiene una o más situaciones relacionadas con los conceptos vistos en clase.

Para cada pregunta debes:
1) Identificar a qué se refiere la observación
2) Explicar si es o no un error y por qué
3) Proponer la corrección

Nota: Responde 5 de las 9 preguntas (elige libremente).


---

## Pregunta 1

Archivo: `RetoEdificioBase.java` (Reto 003)

```java
final int PLANTAS = 8;
for (int dia = 1; dia <= 7; dia++) {
    for (int hora = 1; hora <= 24; hora++) {
        // ...
        for (int planta = PLANTAS - 1; planta >= 0; planta--) {
            // ... planta == 0 como planta baja
        }
    }
}
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `RetoEdificioBase.java` (Reto 003)

```java
if (persianaAbierta) {
    ventana = "[ ]";
} else if (luzEncendida) {
    ventana = "[*]";
} else {
    ventana = "[º]";
}
System.out.print(ventana + ":");
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `RetoEdificioExtendido.java` (Reto 003)

```java
int[] consumoPorDia = new int[8];
for (int dia = 1; dia <= 7; dia++) {
    // ...
    consumoPorDia[dia] += consumoHora;
}
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `RetoEdificioExtendido.java` (Reto 003)

```java
boolean hayMantenimiento = random.nextDouble() < 0.05;
int plantaMantenimiento = hayMantenimiento ? (1 + random.nextInt(7)) : -1;
// ...
if (planta == plantaMantenimiento) {
    ventana = "[#]";
}
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `RetoEdificioExtendido.java` (Reto 003)

```java
System.out.println("CONSUMOS: ");
for (int d = 1; d <= dia; d++) {
    System.out.print("D" + d + ": " + consumoPorDia[d] + " | ");
}
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `RetoEdificioBase.java` (Reto 003)

```java
try {
    Thread.sleep(300); // Pausa para ver el cambio (opcional)
} catch (InterruptedException e) {
    e.printStackTrace();
}
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `RetoEdificioExtendido.java` (Reto 003)

```java
int[] consumoPorDia = new int[8];

for (int dia = 1; dia <= 7; dia++) {
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `RetoEdificioExtendido.java` (Reto 003)

```java
if (rayoCayo && hora == 8) {
    System.out.println(" Un rayo ha inutilizado la columna " + columnaAveriada);
}
if (hayMantenimiento && hora == 8) {
    System.out.println(" Planta " + plantaMantenimiento + " en mantenimiento");
}
```

¿Qué observas en este código?

---

## Pregunta 9

Archivo: `RetoEdificioExtendido.java` (Reto 003)

```java
if (persianaAbierta) ventana = "[ ]";
else if (luzEncendida) {
    ventana = "[*]";
    consumoHora++;
} else ventana = "[º]";
```

¿Qué observas en este código?

---

## Criterios de evaluación

- Identificación correcta del error: 40%
- Explicación del porqué es un error: 30%
- Propuesta de corrección válida: 30%

