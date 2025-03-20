# Laboratorio1-Multiplataforma-Cesar Rafael Gonzales Tucto

void main() {
  List<int> numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  

  List<int> numerosPares = numeros.where((numero) => numero.isEven).toList();
  List<int> numerosImpares = numeros.where((numero) => numero.isOdd).toList();
  
  int sumaPares = numerosPares.reduce((value, element) => value + element);
  int sumaImpares = numerosImpares.reduce((value, element) => value + element);
  
  int menorNumero = numeros.reduce((value, element) => value < element ? value : element);
  int mayorNumero = numeros.reduce((value, element) => value > element ? value : element);
  

  print('La suma de los números pares es: $sumaPares');
  print('La suma de los números impares es: $sumaImpares');
  print('El menor número es: $menorNumero');
  print('El mayor número es: $mayorNumero');
}

