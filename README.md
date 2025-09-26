# Parcial de Programación I (Java) — Versión B

> **Duración:** 90 minutos
> **Lenguaje:** Java (JDK 17+)
> **Modalidad:** Individual, sin internet ni IA
> **Ejecución:** Por consola

---

## Instrucciones generales

* Usa `Scanner` para leer desde teclado.
* Valida entradas **numéricas** y controla la **división por cero** cuando aplique.
* Imprime exactamente lo solicitado; cuida mayúsculas, espacios y saltos de línea.
* Entrega un proyecto con la siguiente estructura:

```
/Codigo_ApellidoNombre/
  src/
    Ejercicio1.java
    Ejercicio2.java
    Ejercicio3.java   (opcional)
```

**Puntaje:**

* Ejercicio 1 (35 pts)
* Ejercicio 2 (35 pts)
* Ejercicio 3 opcional (hasta +10 pts)
* Estilo/validaciones (20 pts)

**Criterios de calificación (resumen):** Correctitud (60%), validaciones (15%), claridad/estilo (15%), pruebas mínimas mostradas en consola (10%).

---

## Ejercicio 1 (35 pts)

**Enunciado**
Solicita **dos números reales** `x` y `y`.

* Si `x >= y`: muestra la **suma** (`x + y`) y la **diferencia** (`x - y`).
* Si `x < y`: muestra el **producto** (`x * y`) y la **división** (`x / y`, del **primero respecto al segundo**).
* Si debes dividir y `y == 0`, imprime: `No se puede dividir entre cero` y **no** intentes la división.

**Ejemplos de ejecución:**

```
Entrada:
x=7
y=7
Salida:
Suma: 14.0
Diferencia: 0.0
```

```
Entrada:
x=4
y=8
Salida:
Producto: 32.0
Division (x/y): 0.5
```

---

## Ejercicio 2 (35 pts)

**Enunciado**
Pide **tres notas** `a`, `b`, `c` en escala **0.0–10.0**. Calcula el **promedio** con dos decimales y muestra:

* `Promocionado` si **promedio ≥ 7.0**
* `Regular` si **4.0 ≤ promedio < 7.0**
* `Reprobado` si **promedio < 4.0**

**Validación:** cada nota debe estar en `[0.0, 10.0]`. Si alguna no lo está, imprime `Nota invalida` y **termina** el ejercicio.

**Ejemplo:**

```
Entrada:
7.0, 6.9, 8.0
Salida:
Promedio: 7.30
Estado: Promocionado
```

**Sugerencia de formato (opcional):**

```java
System.out.printf("Promedio: %.2f%n", promedio);
```

---

## Ejercicio 3 — Opcional (+10 pts)

**Enunciado**
Declara tres vectores `A`, `B`, `C` de **cinco enteros** cada uno.

* Pide 5 valores para `A` y 5 para `B`.
* Calcula `C[i] = A[i] + B[i]`.
* Muestra `A`, `B`, `C` (una línea por vector) y además la **suma total** de los elementos de `C` como `Suma(C): <valor>`.

**Ejemplo:**

```
A: 10 0 -5 2 3
B:  1 2  5 8 1
C: 11 2  0 10 4
Suma(C): 27
```

**Sugerencia (lectura de arreglos):**

```java
int[] v = new int[5];
for (int i = 0; i < 5; i++) v[i] = sc.nextInt();
```

---

## Casos de prueba mínimos recomendados

* **Ej1:** casos `x > y`, `x < y`, `x == y`, y división con `y = 0`.
* **Ej2:** valores en los límites (0.0 y 10.0), una nota fuera de rango, y un caso para cada categoría.
* **Ej3 (opcional):** vectores con positivos, negativos y ceros; verificación de la suma total de `C`.

---

## Buenas prácticas esperadas

* Nombres descriptivos (`promedio`, `estado`, `sumaTotal`).
* Mensajes de salida claros y consistentes con los ejemplos.
* Comentarios **breves** sobre bloques no triviales.

---

¡Éxitos! ✨