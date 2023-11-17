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