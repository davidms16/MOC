# Reflexión — MiniApp de Biblioteca (POO en PHP)

**Nombre:** David Menéndez Santos.

## 1. Encapsulación: ¿por qué los atributos de `MaterialBiblioteca` son `private`? Pon un ejemplo de bug que evitarías.

Los atributos de MaterialBiblioteca son private porque asi solo esa misma clase y aquellas que hereden estos atributos podran editarlos, y da un aspecto mas "profesional" al tener todos los atributos futuramente usados en una misma clase que luego otras heredaran.

## 2. Herencia: ¿qué ventaja tiene que `Libro`, `Revista` y `DVD` hereden de `MaterialBiblioteca`?

Tiene la ventaja de que no hay que volver a formar los atributos, por lo que directamente al solo haber un tipo de atributo hay un tipo de dato, y no se formaran en el proceso duplicados de datos o directamente se actualizaran atributos que no deberian, rompiendo el proceso.

## 3. Polimorfismo: explica qué pasa cuando el `foreach` del catálogo llama a `$m->mostrarFicha()` sin saber el tipo.

Usando polimorfismo, el mismo codigo sabe que tipo de atributo usar.

## 4. Interfaces: ¿qué diferencia hay entre `Prestable` (interfaz) y `Loggable` (trait)? ¿Cuándo usarías cada uno?

La diferencia principal es que Prestable, al ser una interfaz, tiene metodos no definidos los cuales se implementan en una clase al añadir la interfaz a esta, mientras que Loggable, al ser un trait, tiene ya los metodos definidos. Lo suyo seria usar la interfaz cuando se necesita usar un metodo en especifico en multples ocasiones, alterando el codigo en la clase en la que se añada, mientras que el trait se usaria cuando se quiere reusar el codigo especifico.

## 5. Repositorio: ¿por qué el SQL está en `MaterialRepo` y no dentro de `Libro`?

Lo que entiendo es que se hidrata un objeto vacio con los datos de la base de datos en el repositorio, debido a que el respositorio puede acceder a los datos de la base de datos mientras que los de fuera "no saben SQL", por lo que no pueden sacar los datos de ahi.

## 6. Integración: ¿cómo se relacionan los objetos con `$_SESSION['user']` en `prestar.php`?

Se relaciona en base a los datos necesarios, como el material_id, el id del user, o el titulo.

## 7. Java vs PHP: cita tres diferencias concretas que hayas notado.

El uso de $ en vez del tipo de dato especifico, el require_once, y el uso de -> en vez de "."

## 8. Diseño: si mañana añadieras `Mapa` como nuevo tipo, ¿qué archivos tocarías?

_(sin responder)_

## Ampliaciones resueltas

Marcadas: ninguna

_(sin documentar)_

## Autoevaluación

_(sin rellenar)_
