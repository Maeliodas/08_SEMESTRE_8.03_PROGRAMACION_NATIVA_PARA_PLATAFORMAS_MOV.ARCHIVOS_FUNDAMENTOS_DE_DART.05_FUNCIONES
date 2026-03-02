Quinto archivo hecho con dart, esta vez funciones, este es el codigo
```dart
void main(){
  print(greetEveryone());
  print('Suma: ${addTwoNumbers(3, 6)}'); //Se requieren valores posicionales, es decir, el primer valor va para la primera variable y el segundo para la segunda
  print('Suma opcional: ${addTwoNumbersOptional(9)}');
  print(greetPerson(name : 'Victor')); //para pasarlos a nombrados debemos ponerle (nombrevariable=valor), quitamos mensaje para que use el predeterminado
}

/*//Definimos una funcion
String greetEveryone(){
  return 'Hello everyone';
}*/

//Funcion con la flecha (valor unico)+
String greetEveryone() => 'Hello everyone!';

//Pasar parametros a funcion definiendo tipo de datos
int addTwoNumbers(int a, int b) => a + b;

//Pasando por opcionales se pone entre [] para indicar que es nula junto al ? y su validación, si quitamos [] la validación debe quedar
int addTwoNumbersOptional(int a, [int b = 0 /podemos asignar un valor directamente/]){
  //b = b ?? 0;
  //b ??= 0; //Equivalente a la linea anterior
  
  return a + b;
} 

//Para recibir caracteres con posicional para ser nombrados, deberemos poner los parametros en {} para volverlos obligatorios usamos required, si queremos un valor opcional, quitamos required y asiganamos valor por defecto
String greetPerson({required String name,  String message = 'Hola'}){
  return '$message $name';
}
```
Este codigo nos permite mostrar las distintas formas de trabajar con funciones en Dart y cómo manejar parámetros obligatorios, opcionales y nombrados.
