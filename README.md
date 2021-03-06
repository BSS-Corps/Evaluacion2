# Evaluacion2
## Pregunta 1
### Resolución Sofia Poma
En la fase1, en el arhivo Flight el codigo de cobertura solo
cubre el 87% de los métodos, y el 13% de los metodos
que no son cubiertos son:

-Public String getFlightType()

Además las lineas cubiertas solo estan al 68%, mientras
que el 22% de las lineas no cubiertas son las lineas:
24, 33-38, 51-53.

## Pregunta 2
### Resolución Bruno Cipriano
Teniendo en cuenta que la refactorizacion no arregla errores,
sino que mejora el diseño. John tiene la necesidad de refactorizar
el codigo ya que en el archivo Flight, en el metodo addPassenger()
que se encuentra en la linea 28, usa una estructura condicional
selectiva (switch) lo cual nos hace depedener mucho del campo
flightType además de tener que impletar casos de prueba para cada
tipo de vuelo. 

En lugar de esta estructura, John deberá refactorizar
la funcion aplicando polimorfismo a esta, ya que así no se necesitará
una evaluación flightType como lo hacia con la estructura switch.

## Pregunta 3
### Resolución Sebastian Segundo

### ¿Cual es la cobertura de codigo?
La refactorizacion que hizo John en la fase 3 no afecta 
en la cobertura de codigo pues se sigue cubriendo la misma
cantidad de metodos y lineas que en la fase 2.
### ¿ La refactorización de la aplicación TDD ayudó tanto a mejorar la calidad del código?.
Si, al usar polimorfismo permite generalizar los metodos
de addPassenger y removePassenger lo cual permite estandarizar
las llamadas a los métodos de las entidades de dominio. Además extiende
funcionamiento de estos a través de la sobrecarga de métodos.

## Pregunta 4
### Resolución Bruno Cipriano
La regla de tres está relacionada a la refactorización, esta regla nos ayuda
a decidir cuando se debe refactorizar el código. Si hay código duplicado y
se desea volver a reutilizar ese código entonces se dará la refactorización. 
La regla de 3 también menciona que es mala práctica tener código duplicado, 
pues es dificil de mantener ya que si se desea cambiar este código, se tendrá 
de hacerlo en cada lugar donde el código se repita.
### Resolución Sofía Poma
Jhon tiene conocimiento de la regla de 3 por lo tanto al agregar 
un nuevo tipo de vuelo (PremiumFlight) y luego implementar el test 
de PremiumFlight nota que estaria repitiendo el mismo código que
en el test de BusinessFlight y de EconomyFlight, entonces 
procede a refactorizar las pruebas.

## Pregunta 5
### Resolución Sebastian Segundo
Se implementó un diseño inicial de la clase PremiumFlight
en la carpeta Produccion de la Fase4.

## Pregunta 6
### Resolución Bruno Cipriano
Se implementaron las pruebas de la clase PremiumFlight 
en el AirportTest de la Fase4.

## Pregunta 7
### Resolución Sofía Poma
Se agregó la lógica comercial para pasajeros VIP en la
clase PremiumFlight.

## Pregunta 8
### Resolución Sebastian Segundo
Se agregó la nueva prueba para verificar que un pasajero
solo se puede agregar al vuelo solo una vez.
La ejecución de las pruebas es exitosa con una cobertura
de 100%.

<img src="./recursos/pregunta8_cobertura.jpg">


## Observación:
Profesor, como recordará en clase, mis compañeros Bruno Cipriano y Sofia Poma
no podian abrir el proyecto del repositorio en el IDE, por ello,
usted nos brindó la facilidad de detallar qué pregunta hizo
cada uno en el README.