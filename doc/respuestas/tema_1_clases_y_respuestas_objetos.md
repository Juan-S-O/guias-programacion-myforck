<!--
Posible prompt:
<prompt>
Tengo un cuestionario con preguntas sobre "Clases y Objetos". Debes tener en cuenta que los conocimientos previos que tengo (y por tanto tus respuestas deben ser adaptadas), son:
- C/C++ sin orientación a objetos.
- Temas de Java previos: ninguno.

Cada respuesta debe tener entre 2 - 4 párrafos de longitud (sin contar los trozos de código).

Por favor, escribe en impersonal las respuestas.

</prompt>
----
-->

# TEMA 1. Clases y objetos

## 1. ¿Cuáles son las cuatro características básicas de la programación orientada a objetos? Describe brevemente cada una.

### Respuesta
Las cuatro características básicas de la programación orientada a objetos son **encapsulamiento, herencia, polimorfismo y abstracción**.  

El **encapsulamiento** consiste en agrupar datos y métodos que operan sobre ellos dentro de una unidad llamada clase, limitando el acceso directo a ciertos componentes mediante modificadores de visibilidad. Esto permite proteger los datos y controlar cómo se manipulan desde fuera de la clase.  

La **herencia** permite que una clase nueva, llamada subclase, adopte atributos y métodos de una clase existente, denominada superclase. Esto facilita la reutilización de código y la creación de jerarquías de clases.  

El **polimorfismo** se refiere a la capacidad de un objeto de tomar múltiples formas, normalmente mediante la redefinición de métodos heredados, lo que permite que diferentes objetos respondan de manera distinta a la misma operación.  

Finalmente, la **abstracción** implica representar únicamente los detalles esenciales de un objeto, ocultando la complejidad interna. Esto se logra mediante clases y métodos que proporcionan una interfaz clara para interactuar con el objeto, sin necesidad de conocer su implementación interna. 

## 2. Cita cuatro lenguajes populares que permitan la programación orientada a objetos

### Respuesta
Algunos de los lenguajes más populares que permiten la programación orientada a objetos son **Java, C++, Python y C#**.  

**Java** es un lenguaje completamente orientado a objetos, ampliamente utilizado en aplicaciones de escritorio, móviles y web, y se caracteriza por su portabilidad gracias a la máquina virtual de Java (JVM).  

**C++** es un lenguaje híbrido que permite tanto programación estructurada como orientada a objetos, ofreciendo características como clases, herencia y polimorfismo sobre la base de un lenguaje cercano al hardware.  

**Python** es un lenguaje interpretado y de alto nivel, con soporte completo para programación orientada a objetos, incluyendo clases, herencia múltiple y métodos especiales, lo que facilita el desarrollo rápido y legible.  

**C#** es un lenguaje desarrollado por Microsoft que sigue el paradigma de objetos y se utiliza principalmente en aplicaciones de Windows, videojuegos con Unity y aplicaciones web con .NET, proporcionando un sistema robusto de clases, interfaces y manejo de objetos.


## 3. Los paradigmas anteriores a la POO, ¿Qué es la **programación estructurada**? y, todavía mejor, ¿Qué es la **programación modular**?

La **programación estructurada** es un paradigma que organiza el código en bloques secuenciales, condicionales y de repetición, evitando el uso de saltos incontrolados como `goto`. Este enfoque permite un flujo lógico claro y facilita la comprensión y depuración del programa.  

Por su parte, la **programación modular** es una evolución de la estructurada en la que el código se divide en módulos o funciones independientes que cumplen tareas específicas. Cada módulo puede ser desarrollado, probado y mantenido de manera autónoma, favoreciendo la reutilización y la organización del software.  

Ambos paradigmas se centran en el control del flujo del programa y la separación de responsabilidades, pero carecen de la noción de objetos que caracteriza a la programación orientada a objetos.
### Respuesta

## 4. ¿Qué tres elementos definen a un objeto en programación orientada a objetos?

### Respuesta
Los tres elementos que definen a un objeto en programación orientada a objetos son **atributos, métodos y estado**.  

Los **atributos** representan las propiedades o características del objeto, como valores que describen su identidad.  

Los **métodos** son las funciones o comportamientos que el objeto puede realizar, y permiten interactuar con sus datos o con otros objetos.  

El **estado** se refiere a la combinación de valores actuales de los atributos en un momento dado, que determina cómo se comporta el objeto frente a las operaciones que se le aplican.

## 5. ¿Qué es una clase? ¿Es lo mismo que un objeto? ¿Qué es una instancia? ¿Todos los lenguajes orientados a objetos manejan el concepto de clase?

### Respuesta

Una **clase** es una plantilla o estructura que define los atributos y métodos que tendrán los objetos. No es lo mismo que un objeto: mientras la clase es la definición, el objeto es la instancia concreta de esa definición.  

Una **instancia** es un objeto creado a partir de una clase, con valores específicos para sus atributos. Cada instancia puede comportarse según los métodos definidos en la clase, pero mantener su propio estado independiente de otras instancias.  

No todos los lenguajes orientados a objetos manejan explícitamente el concepto de clase. Por ejemplo, en lenguajes como JavaScript se puede crear objetos directamente sin definir una clase formal, mientras que en Java o C++ la clase es fundamental.

## 6. ¿Dónde se almacenan en memoria los objetos? ¿Es igual en todos los lenguajes? ¿Qué es la **recolección de basura**? 

### Respuesta
Los **objetos** se almacenan en memoria dinámica (heap) en la mayoría de los lenguajes orientados a objetos, aunque la gestión concreta depende del lenguaje. Algunos objetos pequeños o locales pueden almacenarse en stack, pero generalmente el heap permite crear instancias con vida más prolongada.  

No todos los lenguajes manejan la memoria igual; por ejemplo, en C++ el programador puede decidir manualmente dónde crear un objeto, mientras que en Java la memoria se gestiona automáticamente.  

La **recolección de basura** es el proceso mediante el cual el lenguaje identifica objetos que ya no son accesibles desde el programa y libera la memoria que ocupaban, evitando fugas de memoria y optimizando el uso de recursos.

## 7. ¿Qué es un método? ¿Qué es la **sobrecarga de métodos**? 

### Respuesta
Un **método** es una función definida dentro de una clase que describe un comportamiento que los objetos de esa clase pueden realizar. Permite manipular atributos y realizar operaciones sobre la instancia del objeto.  

La **sobrecarga de métodos** consiste en definir múltiples métodos con el mismo nombre pero con diferente lista de parámetros dentro de la misma clase. Esto permite que un método se comporte de manera distinta según el tipo o número de argumentos recibidos.


## 8. Ejemplo mínimo de clase en Java, que se llame Punto, con dos atributos, x e y, con un método que se llame `calculaDistanciaAOrigen`, que calcule la distancia a la posición 0,0. Por sencillez, los atributos deben tener visibilidad por defecto. Crea además un ejemplo de uso con una instancia y uso del método

### Respuesta
A continuación se muestra un ejemplo mínimo de la clase `Punto` en Java, con dos atributos `x` e `y`, un método `calculaDistanciaAOrigen` y un ejemplo de uso:

```java
// Definición de la clase Punto
class Punto {
    int x; // atributo x
    int y; // atributo y

    // Método que calcula la distancia desde el punto al origen (0,0)
    double calculaDistanciaAOrigen() {
        return Math.sqrt(x * x + y * y);
    }
}

// Clase con el método main para probar Punto
public class Main {
    public static void main(String[] args) {
        // Crear una instancia de Punto
        Punto p = new Punto();
        p.x = 3;
        p.y = 4;

        // Usar el método calculaDistanciaAOrigen
        double distancia = p.calculaDistanciaAOrigen();
        System.out.println("Distancia al origen: " + distancia);
    }
}
```


## 9. ¿Cuál es el punto de entrada en un programa en Java? ¿Qué es static y para qué vale? ¿Sólo se emplea para ese método main? ¿Para qué se combina con final?
### Respuesta
El punto de entrada en un programa Java es el método `public static void main(String[] args)`. Esta firma concreta permite a la máquina virtual localizar el método sin necesidad de instanciar ningún objeto, ya que debe ejecutar el código inicial de forma independiente a las clases que intervengan después. La estructura del método es rígida porque la JVM lo invoca directamente.

La palabra clave *static* indica que un método o atributo pertenece a la clase y no a una instancia concreta. Esto permite utilizarlo sin necesidad de crear un objeto, lo que resulta esencial para el método `main`. Sin embargo, su uso no se limita a este caso: se emplea en utilidades, constantes de clase y en métodos que no dependen del estado de un objeto.

La combinación *static final* suele emplearse para definir constantes cuyo valor no debe modificarse. El modificador *final* garantiza que el valor asignado no cambie, y al combinarlo con *static* se consigue que la constante sea única y accesible desde cualquier parte sin necesidad de instanciar la clase.

---

## 10. Intenta ejecutar un poco de Java de forma básica… ¿Cómo podemos compilar y ejecutar el programa desde línea de comandos? ¿Java es compilado? ¿Qué es la máquina virtual? ¿Qué es el byte-code y los ficheros .class?
### Respuesta
Un programa Java se compila desde la línea de comandos utilizando `javac`. Por ejemplo, `javac Main.java Punto.java` genera los archivos `.class` correspondientes. Estos archivos contienen *bytecode*, que es un conjunto de instrucciones intermedias independientes de la plataforma. Para ejecutar el programa, se utiliza el comando `java Main`, sin la extensión `.class`.

Java puede considerarse un lenguaje compilado e interpretado. Primero se compila a *bytecode*, y luego la máquina virtual Java (JVM) interpreta o compila dinámicamente estas instrucciones a código nativo mediante optimizaciones como la compilación JIT (*Just In Time*). Esto permite la portabilidad del código entre diferentes sistemas operativos.

La *máquina virtual* actúa como intermediaria entre el programa y el sistema real. Gracias a ella, el mismo archivo `.class` puede ejecutarse en cualquier plataforma que tenga una JVM compatible. El bytecode es precisamente el formato portable que la JVM entiende y ejecuta, lo que diferencia a Java de otros lenguajes más acoplados al hardware.

---

## 11. En el código anterior de la clase Punto: ¿Qué es new? ¿Qué es un constructor? Ejemplo de constructor en una clase Empleado
### Respuesta
La palabra clave `new` sirve para crear una nueva instancia de una clase en el heap. Al ejecutar `new`, la JVM reserva memoria para el objeto y devuelve una referencia al mismo. Durante este proceso, se invoca automáticamente un *constructor*, que es un método especial encargado de inicializar el estado del objeto recién creado.

Un constructor tiene el mismo nombre que la clase y no especifica tipo de retorno. Puede recibir parámetros para inicializar los atributos del objeto de forma personalizada. Si no se declara ningún constructor, Java genera uno por defecto sin argumentos. A continuación se muestra un ejemplo:

```java
class Empleado {
    private final String dni;
    private String nombre;
    private String apellidos;

    public Empleado(String dni, String nombre, String apellidos) {
        this.dni = dni;
        this.nombre = nombre;
        this.apellidos = apellidos;
    }
}
```
## 12. ¿Qué es la referencia this? ¿Se llama igual en todos los lenguajes? Pon un ejemplo del uso de this en la clase Punto
### Respuesta
La referencia *this* se utiliza dentro de los métodos y constructores para señalar al objeto actual. Cuando un atributo y un parámetro comparten el mismo nombre, *this* permite diferenciar entre ambos, evitando ambigüedades durante la asignación. También se emplea para acceder de forma explícita a métodos de la propia instancia.

Aunque el concepto existe en casi todos los lenguajes orientados a objetos, no siempre se llama igual. En C++ aparece como `this` pero es un puntero, mientras que en Python se utiliza el parámetro `self`, que debe escribirse de forma explícita en los métodos. En C#, igual que en Java, se mantiene el término `this`.

```java
class Punto {
    double x;
    double y;

    Punto(double x, double y) {
        this.x = x;  // evita confusión con el parámetro
        this.y = y;
    }
}
```


## 13. Añade ahora otro nuevo método que se llame distanciaA, que reciba un Punto como parámetro y calcule la distancia entre this y el punto proporcionado
### Respuesta
Para calcular la distancia entre dos puntos, se utiliza la fórmula de distancia euclídea en dos dimensiones. El método distanciaA recibe como parámetro otro objeto de tipo Punto y realiza la operación empleando sus coordenadas. El uso de *this* permite dejar claro que los valores de partida corresponden al objeto que invoca el método.

El método devuelve un valor numérico con la distancia resultante. Esta forma de modelar el comportamiento ayuda a encapsular una operación propia de los puntos en el plano, manteniendo el sentido de cohesión dentro de la clase.

```java
class Punto {
    double x;
    double y;

    double distanciaA(Punto otro) {
        double dx = this.x - otro.x;
        double dy = this.y - otro.y;
        return Math.sqrt(dx * dx + dy * dy);
    }
}
```


## 14. El paso del Punto como parámetro a un método, ¿es por copia o por referencia?, ¿afectan los cambios al objeto fuera del método?, ¿qué ocurre con un entero?
### Respuesta
Java emplea siempre paso *por valor* para cualquier parámetro. En el caso de los objetos, lo que se pasa por valor es la referencia, no el objeto en sí. Esto implica que tanto el método como el código llamador comparten acceso al mismo objeto en memoria. Por ello, si dentro del método se modifican los atributos del objeto pasado como parámetro, estos cambios serán visibles fuera del método.

Cuando se pasan tipos primitivos como un *int*, el valor copiado es el dato literal. Al intentar modificar ese valor dentro del método, la variable original que está fuera no se ve afectada. De esta forma, los cambios realizados sobre parámetros primitivos quedan completamente aislados dentro del ámbito local del método.

---

## 15. ¿Qué es el método toString() en Java? ¿Existe en otros lenguajes? Pon un ejemplo de toString() en la clase Punto
### Respuesta
El método `toString()` se encuentra definido en la clase base Object y su función es proporcionar una representación textual del objeto. Dado que la implementación por defecto suele mostrar poca información útil, es habitual sobrescribirlo para mostrar datos significativos del estado del objeto. Este método también se invoca automáticamente cuando un objeto se imprime por consola o se concatena con una cadena.

Muchos lenguajes incluyen mecanismos equivalentes. En C# existe `ToString()`, en Python aparece `__str__()`, y en C++ se recurre normalmente a la sobrecarga del operador `<<` para integrarlo con los streams de salida. Todos ellos comparten el objetivo de facilitar la visualización clara del contenido de un objeto.

```java
class Punto {
    double x;
    double y;

    @Override
    public String toString() {
        return "(" + x + ", " + y + ")";
    }
}
```

## 16. Reflexiona: ¿una clase es como un struct en C? ¿Qué le falta al struct para ser como una clase y las variables de ese tipo ser instancias?
### Respuesta
Un `struct` en C únicamente permite agrupar datos bajo un nombre común, pero no incorpora las características propias de la programación orientada a objetos. Carece de elementos como *encapsulación*, métodos asociados al tipo, control de visibilidad o inicialización automática mediante constructores. Por ello, un struct puede considerarse solo como un contenedor de datos sin comportamiento integrado.

Para que un struct se comportara como una clase, debería permitir integrar funciones internas que actuaran como métodos y proporcionar mecanismos que protegieran el acceso a sus campos. También necesitaría soportar herencia y polimorfismo, lo que permitiría modelar relaciones entre tipos y adaptar comportamientos en función del contexto. Su diseño actual está orientado a la programación estructurada, no a la orientada a objetos.

---

## 17. Quitemos un poco de magia a todo esto: ¿cómo se podría “emular”, con struct en C, la clase Punto con su función para calcular la distancia al origen? ¿Qué ha pasado con this?
### Respuesta
En C, puede emularse parcialmente el comportamiento de una clase utilizando un `struct` para almacenar los datos y funciones externas que operen sobre un puntero a ese struct. El puntero pasado como argumento cumple el papel equivalente a *this*, ya que indica sobre qué objeto se ejecuta la función. Esta aproximación permite organizar código de manera similar, aunque sin integración directa entre datos y comportamiento.

Este método muestra cómo lenguajes orientados a objetos vinculan internamente métodos a las instancias. Sin embargo, en C este vínculo siempre debe hacerse de forma manual, lo que evidencia la ausencia de encapsulación y otras características propias de la orientación a objetos. Aun así, es una técnica útil para comprender cómo se construyen abstracciones más complejas a partir de herramientas básicas del lenguaje.

```c
typedef struct {
    double x;
    double y;
} Punto;

double distancia_al_origen(const Punto* p) {
    return sqrt(p->x * p->x + p->y * p->y);
}

double distancia_a(const Punto* p, const Punto* otro) {
    double dx = p->x - otro->x;
    double dy = p->y - otro->y;
    return sqrt(dx * dx + dy * dy);
}
```