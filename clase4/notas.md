# Clase 4
Cuando un metodo o alguna variable lleva la palabra reservada **static** se indica que dicho metodo o variable es de clase por lo cual no necesita de una instancia para llamarlo.
Por lo que podriamos hacer algo como lo siguiente:

```java
NombreClase.metodo();
NombreClase.variable;
```

La palabra **@Override** antes de un metodo, indica que el metodo ya preestablecido (Regularmente de aquellos que estan heredados de otra clase, un ejemplo son los de la clase Object) sera sobreescrito.

Los metodos staticos no requieren información de la instancia, es decir, no importa lo que pase con el objeto, estos metodos y variables deben manejar información un tanto ajena a los mismos.

Java permite generar bloques de condigo estaticos, estos se ejecutan a la de a webo. La declaración de un bloque estatico es la siguiente:
```java
static {
	/*Codigo que deseamos que se ejecute en esta sección de la clase*/
}
```

Control de acceso = La manera en que vas a definir quien puede ver, a que puede acceder y desde donde puede acceder a todo lo que estas haciendo.

**Modificadores de acceso**

| Modificador        | Clase | Paquete | Subclase | Todos |
|--------------------|-------|---------|----------|-------|
| public             | Si    | Si      | Si       | Si    |
| protected          | Si    | Si      | Si       | No    |
| Vacio (No modifier)| Si    | Si      | No       | No    |
| private            | Si    | No      | No       | No    |

Encapsular es unir comportamientos de diferentes objetos en un solo objeto, una forma de encapsular es la creación de paquetes.

