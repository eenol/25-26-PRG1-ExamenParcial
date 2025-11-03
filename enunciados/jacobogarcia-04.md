# Examen Parcial - jacobogarcia-04

**Usuario GitHub:** jacobogarcia-04
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

Archivo: `Edificio.java` (Reto 003)

```java
for (int horas = 0; horas <= 24; horas++) {
    // ...
    System.out.println("Son las " + horas + ":00 del dia " + dia);
}
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `Edificio.java` (Reto 003)

```java
final String VENTANA_CERRADA = ":[ ]:";
final String VENTANA_LUZ_APAGADA = ":[º]:";
final String VENTANA_LUZ_ENCENDIDA = ":[*]:";
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `Edificio.java` (Reto 003)

```java
System.out.print(
    !persianaAbierta ? VENTANA_CERRADA
                     : luzEncencida ? VENTANA_LUZ_ENCENDIDA : VENTANA_LUZ_APAGADA);
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `Edificio.java` (Reto 003)

```java
if (columna == 3) {
    System.out.print(SEPARADOR);
}
// ...
System.out.print("- P" + (PLANTA_MAXIMA + 1 - planta));
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `Edificio.java` (Reto 003)

```java
final String PARTE_DEABJO_DEL_TECHO = "  |    |    |  |####|  |    |    |  ";
final String BORDE_SUPERIOR_TEJADO = "====================================";
// ...
final String BORDE_INFERIOR_3 = " ==================================";
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `Reto_002.java` (Reto 002, líneas 4-10)

```java
int VIDA_GUERRERO = 20;
final int DAÑO_HACHA_GUERRERO = 2;
final double PORCENTAJE_EXITO_GUERRERO = 0.5;

int VIDA_VAMPIRO = 10;
final int DAÑO_MORDIDA_VAMPIRO = 4;
final double PORCENTAJE_EXITO_VAMPRIO = 0.5;
```

**¿Qué errores encuentras en este código?**

---

## Pregunta 7

Archivo: `ClasificacionConductor.java` (Ejercicios, líneas 19-25)

```java
if (edadDelusuario < MENOR_EDAD) {
    System.out.println("Eres menor de edad, " + DENEGADO);
}

if (edadDelusuario >= MENOR_EDAD) {
    if (licenciaConducir == false) {
        System.out.println("No tienes licencia," + DENEGADO);
    }
```

**¿Cómo mejorarías este código?**

---

## Pregunta 8

Archivo: `ClasificacionEdad.java` (Ejercicios, línea 7)

```java
final int PRIERA_INFANCIA = 5;
```

**Identifica y corrige todos los errores en esta línea.**

---

## Pregunta 9

Archivo: `AdivinadorNumeros.java` (Ejercicios, línea 8)

```java
final int NUMERO_MAXIMO = 100;
final int NUMERO_MINIMO = 1;
Scanner Scanner = new Scanner(System.in);
int numeroPensado = (int) (Math.random() * NUMERO_MAXIMO) + 1;
```

¿Qué observas en este código?

---

## Pregunta 10

Archivo: `CambioDeDinero.java` (Reto 001, fragmento)

```java
int cambio = montoEntregado - montoApagar;
int nuevoCambio;

int cantidad = cambio / billete_100;
nuevoCambio = cambio % billete_100;

cantidad = nuevoCambio / billete_50;
nuevoCambio = nuevoCambio % billete_50;

cantidad = nuevoCambio / billete_20;
nuevoCambio = nuevoCambio % billete_20;
```

**Analiza este código:**

a) ¿Qué problema encuentras con las variables?

b) Reescribe el fragmento mejorándolo.

c) ¿Cómo nombrarías mejor la variable que representa lo que queda por devolver?

---

## Criterios de evaluación

- Identificación correcta del error: 40%
- Explicación del porqué es un error: 30%
- Propuesta de corrección válida: 30%

