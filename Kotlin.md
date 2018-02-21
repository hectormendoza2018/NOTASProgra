# Kotlin

## Variables


### val

- solo de lectura como final, es una constante

## String

### Para saber si dos cadenas son iguales es sensible a la caja
- equals ej nombre1.equals(nombre2) 

### Se desactiva la sensibilidad a la caja por defecto es false
- ej. nombre.equals(nombre, true)

## If

### Uso de if y tomar el resultado
```java
result=if(num1>num2)
	num1
else
	num2
```

## Null

### Para definir un campo o variable nullable se usa el signo de interrogacion ? ejemplo
```java
var str:String? = null
var alien: Alien? =Alien()
```
### Para mostrar un campo o variable definda como nullable
str?.length

## CodeSnippet

### Función main
```java
fun main(args: Array<String>)
```

### Ejemplos de funciones
```java
fun sumar(a:Int, b:Int): Int{
	return a+b
}

fun sumar(a:Int, b:Int) = a + b
```

### Clase
```java
class Persona
```

### Clase con constructor nombre: get edad: get/set
```java
class Persona(val nombre:String, var edad:Int)
```

### Instanciar clase
```java
val persona=Persona("Pedro", 15)
```

### Clase de enumeración
```java
enum class Pais{
	GT, SL, HN, CR, PM
}
```

### Enumeración con un parámetro
```java
enum class Moneda(varl simbolo: String){
	USD("$") PEN("$/.") ART("$")
}
```

### When 
```java
fun numeroALetras(numero:Int)=when(numero){
	1 -> "Uno" 2 -> "Dos"	3 - > "Tres"
	else -> "Error"
}
```

### While
```java
var i=0
while(i<3){			
	println(i)			
}						
							
do{
	println(i)
	i++
}while(i<6)
```

### Rangos			
```java
for(i in 1..10){
	println(i)	
}
```

#### until lo convierte en un intervalo cerrado	
```java
for(i in 1 until 10){
	println(i)
}
```

#### Descendente				
```java
for(i in 20 downtTo 10){
	println(i)
}
```

#### descendente paso 2
```java
for(i in 20 downtTo 10 step 2){
	println(i)
}
```

#### Loop en arreglos
```java
val arreglo=arrayListOf("A", "B", "C")
for(c in arreglo)
	println(c)
```

#### equivalente a downtTo en un rango, ejemplo
```java
var numero=1..15
for(x in numero.reversed()){
	println("$x ")
}
```

#### Acceder al indice del Array los nombres indice y c pueden ser cualquier otros
```java
for((indice, c) int arreglo.withIndex()){
	println("$indice, $c")
}
```

### Crear un TreeMap
```java
var poblacioes=TreeMap<String, Int>()
```

### Agregar elementos a un TreeMap
```java
poblaciones["Guatemala"]=12
```
### Recuperar elementos de un TreeMap
```java
println(poblaciones["Guatemala"]
```
