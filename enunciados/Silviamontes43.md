# Examen Parcial - Silviamontes43

**Usuario GitHub:** Silviamontes43
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Ejercicios, Reto 002

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

Archivo: `WhacAMole.java` (Ejercicios)

```java
System.out.println ("Donde golpeas (entre 1 y " + NUMERO_CASILLAS + ")"
posicionGolpe =scanner.nextInt();
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `WhacAMole.java` (Ejercicios)

```java
final String AGUJERO="( )";
final String MONIGOTE ="(‘’)";
final String MARTILLO= "[[]]";
final String MONIGOTE_GOLPEADO= "[**]";
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `Batalla.java` (Reto 002)

```java
boolean algunMuerto =false;
// ...
boolean algunMuerto=false;
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `Batalla.java` (Reto 002)

```java
boolean vampiroVivo =vidaVampiro <=0;
if (vampiroVivo) {
    // turno del vampiro
}
// ...
boolean guerreroVivo= vidaGuerrero <=0;
algunMuerto=vidaGuerrero<=0 || vidaVampiro <=0 ;
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `Batalla.java` (Reto 002)

```java
} while (!algunMuerto);
String elGanador = vidaGuerrero >0 ? "Guerrero" : "Vampiro";
System.out.println ("Ganó el " + elGanador);
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `CalculadoraDeCambio` (Reto 001)

```java
dineroPorDevolver=cdineroPorDevolver %100;
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `CalculadoraDeCambio` (Reto 001)

```java
String salida;
salida = "Se devuelven";
salida=billetesDe200> 0 ? "y"+ billetesDe200+ "billete(s) de 200" : "";
salida=salida+(billetes100>0? "y" +billetes100 +"billete(s) de 100": "");
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `CalculadoraPrecio` (Reto 001)

```java
import java.util.Scanner;
class CalculadoraPrecio{
    public static void main (String [] args)
    Scanner scanner =new Scanner (System.in);
    final int DESCUENTO_DEL_15=15;
```

¿Qué observas en este código?

---

## Pregunta 9

Archivo: `ConversorDuracion` (Reto 001)

```java
System.out.println ("¿Cuántos segundos desea convertir?");
int totalSegundos= scanner.nextLong();
int dias=totalSegundos /86400;
int horas =(totalSegundos %86400) /3600;
int minutos =(totalSegundos%3600)/60;
int segundos= (totalSegundos&60);
```

¿Qué observas en este código?

---

## Pregunta 10

Archivo: `Batalla.java` (Reto 002)

```java
boolean algunMuerto =false;
final int DAÑO_ESPADA=2;
int vidaGuerrero =20;
final double PORCENTAJE_EXITO_GUERRERO=0.5;
final int DAÑO_MORDIDA =4;
int vidaVampiro=10;
final double PORCENTAJE_EXITO_VAMPIRO=0.5;
boolean algunMuerto=false;
boolean guerreroVivo= true;
boolean vampiroVivo=true;
int vidaGuerrero = 150;
int vidaVampiro = 60;
```

¿Qué observas en este código?

---

## Criterios de evaluación

- Identificación correcta del error: 40%
- Explicación del porqué es un error: 30%
- Propuesta de corrección válida: 30%

