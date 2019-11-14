# Object House
 
En esta Casa Loca hay muchos objetos. 
De cada cosa nos interesa el precio, si es comida o no, y si es un electrodoméstico o no.

## Sobre las cosas 
En este modelo reducido, vamos a considerar las siguientes cosas que podrían ser interesantes: un lavarropas que vale 20000 pesos, una cama que sale 8000, una tira de asado que sale 350 pesos, un paquete de fideos que sale 50 pesos, y una plancha que vale 1200 pesos. Por las dudas aclaramos: la cama no es un electrodoméstico, la plancha sí.

Implementar, además de los objetos que representan cada cosa, un objeto que represente a la casa, que entienda los siguientes mensajes:
- `comprar(cosa)`: registra que se ha comprado una cosa.
- `cantidadDeCosasCompradas()`: indica ... eso.
- `tieneComida()`: indica si compró algo que es comida al menos una vez.
- `vieneDeEquiparse()`: indica si la _última_ cosa que se compró es un electrodoméstico, o bien vale más de 5000 pesos.
- `esDerrochona()`: indica si el promedio del importe de las cosas es de 6000 pesos o más.
- `cosaMasCara()`: retorna la cosa de la casa de mayor valor.
- `electrodomésticos()`: devuelve un objeto que contiene todas las cosas que son electrodomésticos. 
- `malaEpoca()`: indica si todas las cosas  son comida.
- `queFaltaComprar(lista)`: recibe una lista de cosas y devuelve las cosas de esa lista que aún no tien la casa. <br> 
- `faltaComida()`: indica si hay menos de 2 cosas que son comida.


## Más cosas
Agregar las siguientes cosas que pueden comprarse:
- un kilo de milanesas rebozadas: arranca en 260 pesos, puede cambiar por cualquier otro valor.
- una botella de salsa de tomates: arranca 90 pesos, puede cambiar por cualquier otro valor.
- un microondas: 4200 pesos.
- un kilo de cebollas: 25 pesos.
- una compu: 500 dólares. Para saber el precio en pesos, multiplicar por la cotización del dólar. Agregar un objeto `dolar` al que se le pueda preguntar la `cotizacion()`. 
- un "pack comida" que incluye un plato (que puede ser tira de asado, fideos o milanesas) y un aderezo (que puede ser la botella de salsa de tomates o el kilo de cebollas). Precio: la suma del precio de sus componentes.
- un "pack regalo" que incluye una cantidad arbitraria de componentes. Se considera comida si todos sus componentes son comida, se considera electrodoméstico si al menos uno de los componentes es electrodoméstico. El precio es la suma del precio de todos sus componentes, con un descuento del 20%. 



## Más consultas sobre la casa
Agreguemos algunas consultas más para hacerse a la casa
- `gastoEnComida()`: el precio total de _la comida_ comprada por la casa. O sea, hay que contemplar solamente las cosas que son comida. 
- `hayElectrodomesticosBaratos()`: indica si la casa compró, al menos, un electrodoméstico de menos de 3000 pesos.
- `preciosDeElectrodomesticos()`: una colección con **el precio** de cada electrodoméstico que compró la casa. P.ej. si la casa compró la heladera, la tira de asado, la plancha, el microondas y el kilo de cebollas, entonces el resultado debe ser `[20000, 1200, 4200]`. 
- `nivelEnAumento()`: indica si el precio de la última cosa comprada es el doble del precio de la primera, o más.
- `primeraComidaComprada()`: devuelve la primer cosa que se compró que es comida. 
