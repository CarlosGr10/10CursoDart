# Curso de Dart

## Introducción de Dart 

https://pub.dev/

https://dart.dev/

![](https://i.imgur.com/Wu7Zp62.png)

![](https://i.imgur.com/67Zqo5a.png)

![](https://i.imgur.com/mLpCT7J.png)

## Introducción a DartPad

https://dartpad.dev/

**nuestro primer hola mundo**

```dart
void main() {
  print("Hola mundo !");
}
```

## Variables

![](https://i.imgur.com/7v6eNrb.png)

![](https://i.imgur.com/45ICwB4.png)

[Ejercicios drive](https://drive.google.com/drive/folders/1Mn8TLkmuEjYUZsfHPS78tF0xFhPITfXW)


## Tipos de datos básicos

- Booleanos

```dart
void main() {
  print(".: Programa de booleano :.");
  bool estaSoleado = true;
  
  print(estaSoleado);
}
```

- Números

```dart
void main() {
  print(".: Programa de numeros :.");
  
  int edad = 20;
  double estatura = 1.70;
 
  print(edad);
  print(estatura);
  
}
```

- Cadenas

```dart
  void main() {
  print(".: Programa de cadenas :.");
  String pais = "USA";
  
  print(pais);
}
```

- Colecciones - Listas

```dart
void main() {
  print(".: Programa de colecciones (Listas) :.");
  
  List<String> amigos = ["A","B","C"];
  print(amigos);
  print(amigos[0]);

}
```

## Tipo de datos avanzados

- var

```dart
void main() {
  print(".: Programa de variables :.");
    
  var nombre = "Goku";
  print(nombre);

}
```

- final & const

```dart
void main() {
  print(".: Programa de final y const :.");
    
  const nombre = "Vegeta";
  print(nombre);
  
  final pi = 3.1416;
  print(pi);

}

```

- dynamic

```dart
void main() {
  print(".: Programa de variable dynamic :.");

  dynamic nombre = "Vegeta";
  print(nombre);

  nombre = "Goku";

  nombre = 1.37;
  
  print(nombre);

}
```

![](https://i.imgur.com/8jm7fHC.png)


## Manipulación de variables

![](https://i.imgur.com/Dw9upRy.png)

- Incremento & Decremento

```dart
void main() {
  
  int edad = 14;
  
  edad++;
  
  print(edad);
  
  edad--;
  
  print(edad);

}

```

## String con Dart

- comentarios

```dart
void main() {
  
  // Comentario
  
  /*
   * Multicomentario
   * /
}
```

- Concatenación 

```dart
void main() {
  
  String nombre = 'Hola';
  
  String pais = 'Mundo';
  
  String texto = nombre +' '+ pais;
  print(texto);
  
}
```

- Interpolación

```dart
void main() {
  
  String nombre = 'Hola';
  
  String pais = 'Mundo';
  
  
  String texto2 = "$nombre $pais";
  
  print(texto2);
  
}

```

- Agregar caracteres especiales


```dart
void main() {
  
  String nombre = 'Hola';
  
  String pais = 'Mundo';
  
  
  String texto2 = "\"$nombre\n $pais\"";
  
  print(texto2);
  
}
```

- Funciones aplicadas a strings

```dart
void main() {
  
  String nombre = 'Hola';
  
  String pais = 'Mundo';
  
  String texto = "$nombre $pais";
  
  print(nombre.toUpperCase());
  print(nombre.toLowerCase());
  
  texto = texto.replaceAll('Hola','Hello');
  print(texto);
  
}

```

## Conversión de tipos

![](https://i.imgur.com/mFJyJ0a.png)

![](https://i.imgur.com/EenLZp3.png)

- De texto a entero

```dart
void main() {
  String texto = '12';
  int numero = int.parse(texto);
  print(numero + 10);
}
```

- De texto a Decimal

```dart
void main() {
  String texto = '12.8';
  double numero = double.parse(texto);
  print(numero + 10);
}

```

# Ejercicio 1


Realiza el programa en el lenguaje de programación Dart con el siguiente resultado:

Buenos días, trabajadores de TRENES CIUDAD PALETA!!!

El día de hoy la temperatura es de 27 grados
centígrados u 80,6 grados Fahrenheit.
El tren se detendrá en las siguientes ciudades: [Plateada, Celeste, Carmín, Azulona]

Los valores del programa serán cambiados todas las mañanas mediante la manipulación del código, pero se requiere lo siguiente:

El nombre de la estación de trenes puede cambiar, pero siempre debe mostrarse en mayúscula.
La temperatura en grados centígrados siempre será entera, pero Fahrenheit puede ser entera o decimal.
La lista de ciudades puede tener 1 o más nombres (cambiar diariamente).
Dentro del código deben estar todas las instrucciones, a modo de comentarios, necesarias para que otro programador sepa cuáles valores cambiar todos los días.


```dart
void main() {
 
 // Variables de mensaje 
 String message = 'Buenos dias, trabajadores de ';
 String nameStation = 'trenes de ciudad paleta 111';
 
 // Variables de clima
 int gradosC = 27;
 double gradosF = 80.6;
  
 // varibles de ciudades
 List<String> cities = ['Toronto','Seattle','New york'];
  
  
 print(message + nameStation.toUpperCase());
 
 print("El día de hoy la temperatura es de $gradosC grados\ncentígrados u $gradosF grados Fahrenheit.\nEl tren se detendrá en las siguientes ciudades: $cities");
  
}

```

## Operaciones

- Aritmeticas

```dart
void main() {
// Operaciones Aritmeticas

/* --------------------
  +  (suma),
  -  (resta),
  /  (division),
  *  (multiplicacion),
  ~/ (div entero),
  %  (residuo)
-------------------- */ 
  
double val1 = 2;
double val2 = 2;
double resultado = val1 % val2;
  
print(resultado);  
  
}

```

- Asignación

```dart
void main () {
  // Operaciones de asignacion
  int val1 = 1;
  int val2 = 2;
  print("$val1 =+ $val2");
  val1 += val2;
  print("$val1");
}
```


- Relacionales

```dart
void main () {
  // Operaciones Relacionales
  String v1 = "Hola";
  String v2 = "Mundo";
  
  bool resultado = v1 == v2;
  
  print("$v1 != $v2 = $resultado");
  
}
```

- Lógicas


```dart
void main () {
  // Operaciones Logicas
  // ||, &&, ! , ?:
  
  bool calor = true;
  bool frio = false;
  
  bool resultado = calor && frio;
  
  print("$frio || $calor == $resultado");
  
}
```


## Condicionales 

- if

```dart
void main () {
  
  int mascotas = 0;
  if(mascotas == 0)
  {
    print("Tienes $mascotas mascotas");
  }
  
}
```

```dart
void main () {
  
  int mascotas = 5;
  if(mascotas != 0)
  {
    print("Tienes $mascotas mascotas");
  }
  
}
```

- else

```dart
void main () {
  
  int mascotas = 5;
  if(mascotas == 0)
  {
    print("Tienes $mascotas mascotas");
  }
  else
  {
    print("Total mascotas: $mascotas");
  }
  
}
```



- If anidados

```dart
void main () {
  
  int mascotas = 1;
  if(mascotas == 0)
  {
    print("Tienes $mascotas mascotas");
  }
  else
  {
    if(mascotas == 1)
    {
      print("Tienes $mascotas mascota =)");
    }
    else
    {
      print("Total mascotas: $mascotas");  
    }
  }
  
}
```

- switch

```dart
void main () {
  
  int mascotas = 2;
  
  switch(mascotas)
  {
    case 0: 
      print("Tienes $mascotas mascotas");
      break;
    case 1: 
      print("Tienes $mascotas mascota =)");
      break;
    default:
      print("Total mascotas: $mascotas");
  }
  
}
```

## Ciclos

- While

```dart
void main () {
  int tazasCafe = 0;
  int max = 3;
  
  while(tazasCafe < max)
  {
    tazasCafe++;
    print("Cantidad de tazas: $tazasCafe");
  }
 
}
```

- Do while

```dart
void main() {
  
  int tazasCafe = 0;
  int max = 3;
  
  do
  {
    tazasCafe++;
    print("Cantidad de tazas: $tazasCafe");
  } while  (tazasCafe < max);
  
}
```

- For

```dart
void main() {
  
  int tazasCafe = 0;
  int max = 5;
  
  for(int i = 0; i < max; i++)
  {
    print("i= $i");
    tazasCafe++;
    print("Cantidad de tazas: $tazasCafe");
  }
  
}
```

## Enumeraciones

Nota: Utilizamos mayusculas en las enumeraciones

```dart
void main() {
  Tiempo time = Tiempo.Soleado;
  
  switch (time)
  {
    case Tiempo.Soleado:
      print("HOY ESTA SOLEADO");
      break;
    case Tiempo.Lluvioso:
      print("HOY ESTA LLUVIOSO");
      break;
    case Tiempo.Despejado:
      print("HOY ESTA DESPEJADO");
      break;
  }
  
}

enum Tiempo { Soleado, Lluvioso, Despejado }

```

# Ejercicio 2

El código fuente de un programa que tenga las siguientes variables:

- Una variable para almacenar el valor 1.
- Una variable para almacenar el valor 2.
- Una lista de valores.
- Una variable para el resultado.
- Una variable que indique el tipo de operación.

Con las siguientes funciones:

Si el tipo de operación es SUMA, el resultado es igual al valor 1 más el valor 2.
Si el tipo de operación es RESTA, el resultado es igual al valor 1 menos el valor 2.
Si el resultado de la resta es negativo, se debe mostrar NEGATIVO en la consola.
Si el tipo de operación es MULTIPLICACIÓN, el resultado es igual al valor 1 por el valor 2.
Si el tipo de operación es MÓDULO, el resultado es igual al valor 1 módulo el valor 2.
Si el tipo de operación es FACTORIAL, el resultado es igual al factorial de valor 1.
Si el tipo de operación es SUMATORIA, el resultado es igual a la suma de todos los valores de la lista de valores.
Si el tipo de operación es PRODUCTO, el resultado es igual a la multiplicación de todos los valores de la lista de valores.
Al finalizar la ejecución del código debe mostrar el siguiente mensaje dónde 12.2 es el resultado de la operación:

El resultado de la operación es: 12.2


## Colecciones

Las colecciones son importantes porque te permiten almacenar un conjunto de valores o elementos que pueden tener alguna propiedad en común y pueden ser recorridos o iterados, básicamente lo que quiere decir esto es que podemos contener muchos valores en una misma “variable” y podemos acceder a cada uno de ellos. Una colección puede estar vacía o contener diferentes elementos, algunos de los tipos de colecciones iterables son List, Set y Map.

![](https://i.imgur.com/FwNjkix.png)

## Coleccion tipo lista

```dart
void main() {
  
  List<String> amigos = [];
  
  amigos = ["A", "B", "C"];
  
  //  PROPIEDADES
  
  print(amigos.isEmpty); // Verifica si esta vacia la lista
  print(amigos.length); // La longitud de la lista
  
  // FUNCIONES
  
  amigos.add("D"); // Agrega a la lista
  
  amigos.remove("A"); // Elimina de la lista
  
  amigos.insert(0,"Z"); // Agrega segun la posicion
  
  for(int i = 0; i < amigos.length ; i++)
  {
    print("amigos[$i] : ${amigos[i]}");
  }
  
}

```

## Colecciones tipo set

![](https://i.imgur.com/dAB4v7j.png)

```dart
void main() {
 Set<String> paises = {};
 paises = {"Mexico","Argentina","Colombia"};
 
 paises.add("Brasil");
  
 print(paises);
 
 for(int i = 0;i< paises.length;i++)
 {
   print(paises.elementAt(i));
 }
  
}

```

## Colecciones tipo mapa

![](https://i.imgur.com/wEaaL0G.png)

```dart
void main() {
  
 Map<String, dynamic> persona = {
   "nombre":"Cool",
    "edad": 12,
   "pais":"mexico",
 };
  
 print(persona.keys);
 print(persona.values);
 
 print(persona["nombre"]);
  
 
  
 if(persona["comida"] == null)
 {
    print("No tiene esta key");  
 }else
 {
   print(persona["comida"]);
 }
  
}
```

## Coleccion de colecciones 

```dart
void main() {
  
 Map restaurant =
 {
   "nombre": "The restaurant",
   "estrellas": [1,2,3,4,5]
 };
  
 if(restaurant["estrellas"] == null)
 {
   print("No hay estrellas");
 }else{
   List<int> estrellas = restaurant["estrellas"];
   print(estrellas);
   
   int suma = 0;
   for(int i = 0; i < estrellas.length;i++){
      suma += estrellas[i];
   }
   
   double promedio = suma / estrellas.length;
   restaurant.addAll({"promedio":promedio});
  
  print(restaurant);
 }
}

```

### Union de colecciones

- Con el metodo addAll

```dart
void main() {
  
 List<String> colores_primarios = ["rojo","amarillo","azul"];
  
 List<String> colores_secundarios = ["morado","verde","naranja"];
  
 colores_secundarios.addAll(colores_primarios);
 
 print(colores_secundarios);
  
}
```

- Con tres puntos dentro de otra lista

```dart
void main() {
  
 List<String> colores_primarios = ["rojo","amarillo","azul"];
  
 List<String> colores_secundarios = ["morado","verde","naranja",...colores_primarios];
  
 
 print(colores_secundarios);
  
}
```

- Declarando una nueva coleccion

```dart
void main() {
  
 List<String> colores_primarios = ["rojo","amarillo","azul"];
  
 List<String> colores_secundarios = ["morado","verde","naranja"];
  

  List<String> colores = [
    ...colores_primarios,
    ...colores_secundarios
  ];
  
  print(colores);
  
}
```


## Flujo dentro de colecciones

- Condicion if dentro de una lista

```dart
void main() {
 
 bool agregarAmarillo = true;
 bool agregarAzul = false;
  
 List<String> colores = [
   "rojo",
   "verde",
   if(agregarAmarillo) "Amarillo",
   if(agregarAzul) "Azul",
 ];
 
  print(colores);

}

```

- Bucle for dentro de una lista

```dart
void main() {
 
 bool agregarAmarillo = true;
 bool agregarAzul = false;
  
 List<String> colores = [
   "rojo",
   "verde",
   "rosa",
   "azul",
 ];
 
 List<String> nuevosColores = [
   "blanco",
   for(int i = 0; i < colores.length;i++) colores[i],
 ];
  
 print(nuevosColores);

}
```

# Ejercicio 3 

Google Maps es una herramienta de Google que permite localizar diferentes tipos de comercios, entre ellos restaurantes.

La información es almacenada en bases de datos no relaciones y puede ser extraído en la siguiente estructura mediante el lenguaje de programación Dart.


```dart
Set restaurantes = {

{
“nombre”: “El novillo alegre”,
“tipo”: “Argentina”,
“calificaciones”: [4, 5, 2, 1, 2]
},

{
“nombre”: “Baires Grill”,
“tipo”: “Argentina”,
“calificaciones”: [3, 1, 3, 5, 5, 2, 3]
},

{
“nombre”: “Mario Brothers”,
“tipo”: “Italiana”,
“calificaciones”: [4, 3, 2, 1, 1]
},

{
“nombre”: “Molto bene”,
“tipo”: “Italiana”,
“calificaciones”: [4, 3, 1, 1, 5]
}

};

```

Un conjunto de restaurantes que no se puede repetir, que contiene varios mapas con nombre, tipo y una lista con calificaciones.

Google requiere que un programador realice un código en Dart para obtener un resumen de la calificación de los diferentes tipos de restaurantes de una zona. Realizando un promedio de las calificaciones por tipo, el resultado debe ser el siguiente.

```dart
Map rating = {
“Italiana”: 3.0,
“Argentina”: 2.5,
“Todos”: 2.77
};

```

Los tipos de comida pueden variar, al igual que las cantidades de la lista de calificación.