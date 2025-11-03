# Examen Parcial - javierrodriguezrobles07-creator

**Usuario GitHub:** javierrodriguezrobles07-creator
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 001, Reto 003

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

Archivo: `CalculadoraDePrecio.java` (Reto 001)

```java
double precioConIva = precioEnEuros * (1 + tipoDeIva / 100.0);
double precioTotalAntesDescuento = precioConIva * cantidadDeArticulos;
double importeRebaja = precioTotalAntesDescuento * rebaja / 100.0;
double precioFinal = precioTotalAntesDescuento - importeRebaja;
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `CoversorSegundos.java` (Reto 001)

```java
class ConversorSegundos {
    // ...
}
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `DevolucionCambio.java` (Reto 001)

```java
final int Billete_100= 100;
final int Billete_50 = 50;
// ...
int Cambio = DineroUtilizado - DineroAPagar;
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `edificio.java` (Reto 003)

```java
class SimulacionHotel {
    public static void main(String[] args) {
        // ...
    }
}
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `edificio.java` (Reto 003)

```java
while (dia <= DIAS) {
    int consumoDia = 0;
    int hora = 0;
    while (hora < HORAS) {
        // ...
        hora++;
    }
}
System.out.println("Media semanal: " + (consumoTotalSemana / 7));
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `edificio.java` (Reto 003)

```java
int p = PLANTAS;
while (p >= 1) {
    System.out.print(":");
    int c = 1;
    while (c <= HABITACIONES) {
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `DevolucionCambio.java` (Reto 001)

```java
final int Billete_100= 100;
final int Billete_50 = 50;
final int Billete_20 = 20;
final int Billete_10 = 10;
final int Billete_5 = 5;
final int Moneda_2 = 2;
final int Moneda_1= 1;
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `DevolucionCambio.java` (Reto 001)

```java
System.out.print("¿Cuanto dinero tienes que pagar?");
int DineroAPagar = scanner.nextInt();
System.out.print("¿Con cuanto vas a pagar?");
int DineroUtilizado = scanner.nextInt();
```

¿Qué observas en este código?

---

## Pregunta 9

Archivo: `edificio.java` (Reto 003)

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

---

## Pregunta 10

Archivo: `ConversorSegundos.java` (Reto 001)

```java
int dias = segundos / DIAS_EN_SEGUNDOS;
segundos = segundos % DIAS_EN_SEGUNDOS;

int horas = segundos / HORAS_EN_SEGUNDOS;
segundos = segundos % HORAS_EN_SEGUNDOS;
```

¿Qué observas en este código?

---

## Criterios de evaluación

- Identificación correcta del error: 40%
- Explicación del porqué es un error: 30%
- Propuesta de corrección válida: 30%

