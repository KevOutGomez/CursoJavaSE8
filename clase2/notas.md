# Clase 2
Los tipos de archivos con los que nos podemos encontrar en el mundo java.
JAR = Java Archive ( Se empaquetan solo los .class sin comprimir nada)
WAR = Mundo Web
EAR = Cosas empresariales
RAR

## Tipos de Variables
**Variable** Localidad de memoria que tiene asociada una nombre y un tipo.
En java existen diferentes tipos de variables. Los datos primitivos de java son:
* String ( Objeto )
* char ( 1 byte )
* int ( 4 byte ) [ -2 147 483 648 , 2 147 483 648 ] Se puede colocar **_** sustituyendo el uso de **,**. Se puede usar la notación cientfica **2.1E12**. Su Wrappet es **Integer**
* long ( 8 byte )
* double ( 4 byte ) Su Wrappet es **Double**
* boolean ( 1 byte ) Su Wrappet es **Boolean**
* short ( 2 byte )
* byte ( 1 byte ) 
Todas las variables primitivas se inicializan con 0.
Todos los tipos primitivos tienen un envolvente tipo Objeto, a estos envolventes se les llama **Wrape**, esto permite que los tipos primitivos puedan ser tratados como Objetos.
Todos los objetos heredan de la clase **Object**, los cuales si no son inicializadas tiene el valor de null.

La sintaxis para inicializar una variable es la siguiente:
**Tipo de variable** *nombre de la variable* = Valor ;

Cuando se crea una variable sin inicialización, la variable existe pero su contenido es nulo.

Uno de los problemas en el manejo de cadenas es el desborde en la memoria, para evitar dicho problema a partir de java 6 se implemento en la máquina virtual de java algo llamado **Caché de cadenas**.

**StringBuilder** clase de java que permite concatenar cadenas sin necesidad de crear una nueva cadena.
Es recomendado el uso de constantes.

Banderas para compilar java:
Se recomienda el uso de rutas absolutas.
La bandera **-d** indica el lugar donde se guardaran las clases generadas
```bash
javac -d [directorio] Archivo.java
```

La bandera **-cp** indica el ClassPath donde java buscará las clases para compilar el programa:
```bash
java -cp [directorio/o archivo jar] Archivo
```
La bandera **-jar** permite correr archivos **.jar**
```bash
java -jar [ubicación del jar]
```

**Manifiesto (MANIFEST.MF)**: En este archivo ubicado en el directorio **META-INF** se indica la indica la clase principal del proyecto, con la siguiente linea:
```text
Main-Class: [Clase Principal]
```

Para crear un archivo jar lo hacemos a traves del siguiente comando:
```bash
jar cfm [NombreJar.jar] META-INF/MANIFEST.MF *.class
```
## Condicionales
En java puede usarse los operadores terciarios, los cuales asignan un valor, su estructura es la siguiente:
```java
[Variable] = [Condición que devuelve un boolean] ? [Asignación si es verdadero] : [Asignación si es falso]
```
## Arrays
Colección de objetos de un mismo tipo.
La sintáxis en la declaración de un array es la siguiente:
```java
Tipo_de_dato [] nombre_array = {valor1, valor2, valor3};
Tipo_de_dato [] nombre_array = new Tipo_de_dato[tamaño_de_array];
```
Los indices de acceso para los arrays comienzan en 0.

## Loops
### For each
La sintáxis de un for each es la siguiente:
```java
String [] arrays = { "Valor1", "Valor2", "Valor3" };
for ( String array : arrays){
	System.out.println(array);
}
```
**break**: Rompe el ciclo
**continue**: La iteración se salta al siguiente elemento.

Por estándar no debe haber mas de 3 anidaciones de ciclos.

## Clases
Una clase esta compuesta de Propiedades y Métodos.
Las Propiedades identifican las caracteristicas de la clase, en tanto que los Métodos se refieren a las acciones que puede realizar dicha clase.

Tipos de Métodos, deben ser nombrados de la siguiente manera:
* **get**: Devuelven algo
* **set**: Modifican algo
* **is/has/constrains**: Devuelven un valor booleano
* **verbo en infinitivo**: Realizan alguna acción

