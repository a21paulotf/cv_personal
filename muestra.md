# Ejemplos de código creado por mi

## Ejemplo HTML
[Repositorio en GitHub](https://github.com/a21paulotf/conference-web)

## Java
```java
import java.util.Scanner;
class ej1{
	public static void main(String[] args){
		Scanner teclado = new Scanner(System.in);
		int pizzas = teclado.nextInt();
		while(pizzas != 0){
			if(pizzas > 0){
				int amigos = teclado.nextInt();
				Double pelea = Double.valueOf(amigos)%Double.valueOf(pizzas);
				int trozos = amigos/pizzas;		
				if(pelea != 0){
					System.out.println("PELEA");
				}else{
					System.out.println(trozos);
				}
			}
		pizzas = teclado.nextInt();
		}
	}
}
```

## Kotlin
```kotlin
fun main() {
    val puntuacion = readln().toInt()
    when (puntuacion) {
        in 90..100 -> print("La calificación es tipo A")
        in 80..90 -> print("La calificación es B")
        in 70..80 -> print("La calificación es C")
        in 0..70 -> print("La calificación es D")
        else -> print("La calificación es F")
    }
}
```

## Powershell
```powershell
function Sumar([Double]$num1, [Double]$num2){
    $resultado = $num1+$num2
    return $resultado
}

function Resta([Double]$num1, [Double]$num2){
    $resultado = $num1-$num2
    return $resultado
}
a
function Multiplicar([Double]$num1, [Double]$num2){
    $resultado = $num1*$num2
    return $resultado
}

function Dividir([Double]$num1, [Double]$num2){
    $resultado = $num1/$num2
    return $resultado
}

[int]$calculo = 5
while($calculo -ne 0){
[int]$calculo = Read-Host "Qué cálculo quieres hacer? Suma(1) Resta(2) Multiplicacion(3) Division(4) Salir(0)"

   
switch($calculo){
    1{
        [Double]$num1 = Read-Host "Dime el valor del numero 1"
        [Double]$num2 = Read-Host "Dime el valor del numero 2"
        Write-host "Resultado: "$(Sumar $num1 $num2)
    }2{
        [Double]$num1 = Read-Host "Dime el valor del numero 1"
        [Double]$num2 = Read-Host "Dime el valor del numero 2"
        Write-host "Resultado: "$(Resta $num1 $num2)
    }3{
        [Double]$num1 = Read-Host "Dime el valor del numero 1"
        [Double]$num2 = Read-Host "Dime el valor del numero 2"
        Write-host "Resultado: "$(Multiplicar $num1 $num2)
    }4{
        [Double]$num1 = Read-Host "Dime el valor del numero 1"
        [Double]$num2 = Read-Host "Dime el valor del numero 2"
        if($num2 -eq 0){
            Write-Host "No se puede dividir entre 0"
        }else{
            Write-host "Resultado: "$(Dividir $num1 $num2)
        }
    }0{
        Write-Host "Saliendo..."
    }default{
        Write-Host "Introduce un número válido"
    }
  }
}
```