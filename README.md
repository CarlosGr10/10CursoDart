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

# Ejercicio


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



