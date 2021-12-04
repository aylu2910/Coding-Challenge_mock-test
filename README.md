# Coding Challenge - Mock test

### 1. Pares e Impares
Deben crear una función llamada paresEimpares que reciba 3 parámetros. Los dos primeros números y el tercero una palabra (string).
La función tiene que mostrar en la consola los números entre el uno y el primer parámetro que recibe pero debe en primer lugar mostrar todos los números pares y luego los impares. 
Además, cuando el número sea divisible por el segundo parámetro pasado a la función, en vez de loggearlo, debe imprimir la palabra que recibe como tercer parámetro. 

Ejemplo:
``` 
paresEImpares(10,7,’prueba’)
2
4
6
8
10
1
3
5
’Prueba’
9
```
### 2. Index o Value? 
Crea una función llamada "min" que tome dos parámetros. Un arreglo de números desordenados y un string que va a valer "index" o "value". Si el string es "value", la función deberá devolver el número más chico del array. Si el string es "index", la función deberá devolver el índice (la posición) del número más chico en el array. 
	Ejemplo:
- min([5,8,2,3,4,9,1,18], "index") debe retornar 6 (porque es el índice del 1 que es el menor)
- min([5,8,2,3,4,9,1,18], "value") debe retornar 1 (porque 1 es el menor número)

### 3. Doble Filtro

Utils:
```
var paises = [
   {
       nombre: "argentina",
   continente: "sudamerica",
   poblacion: 40000000
   },
   {
       nombre: "brasil",
   continente: "sudamerica",
   poblacion: 300000000
   },
   {
       nombre: "venezuela",
   continente: "sudamerica",
   poblacion: 25000000
   },
   {
       nombre: "chile",
   continente: "sudamerica",
   poblacion: 10000000
   },
   {
       nombre: "australia",
   continente: "oceania",
   poblacion: 18000000
   },
   {
       nombre: "nueva zelanda",
   continente: "oceania",
   poblacion: 8000000
   },
   {
       nombre: "china",
   continente: "asia",
   poblacion: 1000000000
   },
   {
       nombre: "tailandia",
   continente: "asia",
   poblacion: 32000000
   },
   {
       nombre: "vietnam",
   continente: "asia",
   poblacion: 23000000
   },
   {
       nombre:"españa",
   continente: "europa",
   poblacion: 29000000
   },
   {
       nombre: "alemania",
   continente: "europa",
   poblacion: 33000000
   },
   {
       nombre: "francia",
   continente: "europa",
   poblacion: 65000000
   },
   {
       nombre: "portugal",
   continente: "europa",
   poblacion: 4000000
   },
   {
       nombre: "grecia",
   continente: "europa",
   poblacion: 12000000
   },
   ]
```
Deben crear una función llamada doubleFilter que reciba como parámetro un arreglo de objetos, un continente, y un número de población. La función filtra el arreglo solo con los países que sean del continente pasado por parámetro, y además, los que su población sea mayor o igual a la del ultimo parámetro. Debera devolver un arreglo con los nombres de los paises de los objetos que cumplan con la condicion. 

### 4. Doble Filtro II

Ahora deben refactorizar la función doubleFilter, que recibirá los mismos tres parámetros pero en vez de devolver un arreglo con los nombres de los países que cumplan con las condiciones, devolverá un objeto con una key ‘nombres’ que tendrá como valor un arreglo con los nombres de los países y otra llamada ‘población total’ cuyo valor sea la suma de las poblaciones de los países filtrados.

Ejemplo:
doubleFilter(paises, "sudamerica", 30000000) debe retornar:
```
{
    nombres: [‘argentina’, ‘brasil],
    poblacion total: 340000000
}
```
### 5. Doble Filtro III

Ahora, la función doubleFilter debe retornar un objeto que, además de tener las keys nombres y población total, tenga una key mayor y una menor en la que guarde el nombre de los países con mayor y menor población respectivamente.

Ejemplo:
doubleFilter(paises, "sudamerica", 30000000) debe retornar:
```
{
    nombres: [‘argentina’, ‘brasil],
    poblacion total: 340000000,
    mayor: ‘brasil’,
    menor: ‘argentina’
}
```
