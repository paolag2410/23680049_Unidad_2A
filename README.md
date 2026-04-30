# Unidad 2: Graficación 2D

La graficación en dos dimensiones (2D) es una rama de la computación gráfica que permite representar objetos en un plano utilizando coordenadas (x, y). Es fundamental en el desarrollo de interfaces gráficas, videojuegos, simulaciones y animaciones. A través de transformaciones geométricas, es posible modificar la posición, tamaño, orientación y forma de los objetos.

## 2.1 Transformación Bidimensional

Las transformaciones bidimensionales son operaciones matemáticas que se aplican a los objetos para modificar sus propiedades en el plano cartesiano.

## 2.1.1 Traslación

La traslación consiste en mover un objeto de una posición a otra sin alterar su forma ni su orientación.

Fórmula:
```
x' = x + dx
y' = y + dy
```
Características:

Mantiene forma y tamaño
No altera la orientación
Es una transformación rígida

## 2.1.2 Escalamiento

El escalamiento permite cambiar el tamaño de un objeto.

Fórmula:
```
x' = x * Sx
y' = y * Sy
```
Características:

Si S > 1 aumenta el tamaño
Si 0 < S < 1 reduce el tamaño
Puede ser uniforme o no uniforme

## 2.1.3 Rotación

La rotación gira un objeto alrededor del origen o de un punto específico.

Fórmula:
```
x' = x cosθ - y sinθ
y' = x sinθ + y cosθ
```
 Características:

Depende del ángulo θ
Puede ser horario o antihorario
Mantiene forma y tamaño

## 2.1.4 Sesgado (Shear)

El sesgado inclina un objeto en una dirección determinada.

Fórmula:
```
x' = x + kx * y
y' = y + ky * x
```
Características:

Deforma la figura
No conserva ángulos
Usado en efectos visuales
2.2 Representación Matricial de las Transformaciones

Las transformaciones se pueden representar mediante matrices, lo que facilita su implementación en programación.

Ejemplo (traslación con coordenadas homogéneas):
```
| x' |   | 1  0  dx |   | x |
| y' | = | 0  1  dy | * | y |
| 1  |   | 0  0  1  |   | 1 |
```
Ventajas:

Permite combinar transformaciones
Simplifica cálculos
Base de gráficos por computadora

Ejercicio sugerido:

Flechas → mover figura
Tecla "+" → escalar
Tecla "R" → rotar
2.3 Trazo de Líneas Curvas

Las curvas permiten representar formas suaves y complejas.

## 2.3.1 Curvas de Bézier

Se definen mediante puntos de control.

Fórmula:

B(t) = (1 - t)^n P0 + n(1 - t)^(n-1)t P1 + ... + t^n Pn

Características:

Suaves y precisas
Control intuitivo
Muy usadas en diseño gráfico

## 2.3.2 B-Spline

Son una extensión de las curvas de Bézier.

Características:

Mayor control local
Más suaves
No pasan por todos los puntos de control

Diferencia clave:

Bézier: control global
B-Spline: control local

Ejercicio sugerido:
Crear una animación donde la curva cambie al mover puntos de control.

## 2.4 Fractales

Los fractales son figuras que presentan autosimilitud, es decir, se repiten a diferentes escalas.

Características:

Estructuras infinitas
Generación recursiva
Alta complejidad visual

Ejemplos:

Conjunto de Mandelbrot
Copo de nieve de Koch

Aplicaciones:

Simulación de naturaleza
Arte digital
Gráficos por computadora
2.5 Uso y Creación de Fuentes de Texto

Las fuentes de texto son conjuntos de caracteres diseñados para representar letras y símbolos.

Tipos:

Vectoriales (TrueType, OpenType)
Mapas de bits

Características:

Escalabilidad
Estilo (negrita, cursiva)
Legibilidad

Creación:

Se diseñan mediante curvas (generalmente Bézier)
Uso de editores de fuentes

Importancia:

Interfaces gráficas
Diseño web
Aplicaciones móviles

## Conclusión

La graficación 2D es una herramienta esencial en la computación moderna. A través de transformaciones, curvas y fractales, se pueden crear representaciones visuales complejas y dinámicas. Además, el uso de fuentes de texto permite mejorar la interacción en sistemas digitales.
