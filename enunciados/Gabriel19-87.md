# Examen Parcial - Gabriel19-87

**Usuario GitHub:** Gabriel19-87
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Ejercicios, Reto 003

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

Archivo: `reto3.java` (Reto 003)

```java
piso += persianasAbiertas[planta][habitacion] ? LUZ_ENCENDIDA
        : (lucesEncendidas[planta][habitacion] ? LUZ_ENCENDIDA : LUZ_APAGADA);
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `reto3.java` (Reto 003)

```java
for (int planta = NUMERO_DE_PLANTAS - 1; planta >= 0; planta--) {
    String piso = "";
    for (int habitacion = 0; habitacion < NUMERO_DE_HABITACIONES; habitacion++) {
        // ...
        if (habitacion < NUMERO_DE_HABITACIONES - 1) {
            piso += "::";
        }
    }
    System.out.println(piso + " - Planta " + (planta + 1));
}
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `AdivinaNumero.java` (Ejercicios)

```java
int numeroSecreto = random.nextInt(NUMERO_MAXIMO) + NUMERO_MINIMO;
// ...
if (numeroUsuario < NUMERO_MINIMO || numeroUsuario > NUMERO_MAXIMO) {
    // ...
}
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `PozoCaracol.java` (Ejercicios)

```java
for (int i = 0; i <= 20; i++) {
    if (i > 20 - metrosAgua) {
        System.out.println("  []~~~~~~~~~~~~~~[] _ __ " + i);
    } else {
        System.out.println("  []:. :. :. :. :.[] _ __ " + i);
    }
}
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `ClasificacionConductor.java` (Ejercicios)

```java
System.out.println("¿Tiene licencia de conducir? (true/false):");
boolean tieneLicencia = sc.nextBoolean();
// ...
// (lógica de clasificación y mensajes)
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `PiedraPapelTijera.java` (Ejercicios)

```java
public static String determinarGanador(String jugadaUsuario, String jugadaPrograma) {
    String resultado = "";

    if (jugadaUsuario.equals(jugadaPrograma)) {
        resultado = "empate";
    } else if (jugadaUsuario.equals("piedra")) {
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `AdivinaNumero.java` (Ejercicios)

```java
System.out.println("¡¡¡FELICIDADES!!! 🎉");
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `AdivinaNumero.java` (Ejercicios)

```java
System.out.println(" Se acabaron los intentos!");
```

¿Qué observas en este código?

---

## Pregunta 9

Archivo: `ClasificacionConductor.java` (Ejercicios)

```java
System.out.println("Ingrese su edad:");
int edad = sc.nextInt();

System.out.println("¿Tiene licencia de conducir? (true/false):");
boolean tieneLicencia = sc.nextBoolean();

// Variables predefinidas
String puedeConducirTxt = "Puede conducir.";
```

¿Qué observas en este código?

---

## Criterios de evaluación

- Identificación correcta del error: 40%
- Explicación del porqué es un error: 30%
- Propuesta de corrección válida: 30%

