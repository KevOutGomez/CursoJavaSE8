# Clase 1 (Introducción a Java)
JRE --> Java Run Enviroment (Permite ejecutar programas en java, contiene la máquina virtual)
JDK --> Java Development Kit (Contiene el JRE, las herramientas y el compilador de java)

### Carateristicas de una clase:
**Clase** = Conjunto de archivos y metodos que estan contenidos en un archivo java, la clase principal pública debe contener nombre del archivo.
* Las clases se escriben en notación Camello, la cual consiste en iniciar con una mayuscúla cada clase.
* Las clases no llevan simbolos raros como _ $ % & etc..
* Las clases no llevan verbos.
* Las clases se escriben en singular.
* Llevan el nombre de algo o cumplen una función.
* Byte code son los archivos que en combinación con el .class se ejecutan en la máquina virtual de java.

### Sintáxis de una clase
```java
public class NombreClase{
// Métodos y Atributos
}
```

**ClassPath** = Ruta a las clases. Rutas de directorio o archivos que indican que librerias necesito para correr y ejecutar programas. No hay necesidad de hacer un linkeo a las librerias para generar las clases. Cuando las librerias no estan en el claspath se obtiene la excepción ClassNotFoundException.

**ClassLoader** = Programa que carga todo

**JNI** = Es quien habla con el sistema operativo

Métodos de acceso --> Setters y Getters
Evitar modificaciones de los metodos y atributos desde afuera de una clase

*El nombre calificado de la clase* es la concatenación del nombre del paquete y del nombre de la clase
El uso de un Paquete tiene como finalidad la creación de un *Namespace* esto con la finalidad de generar grupos de clases.
Para asegurar originalidad en cada paquete es recomendable usar el nombre del dominio de la empresa pero invertido.
Todo el nombre del paquete va en minúsculas¡¡¡
 
