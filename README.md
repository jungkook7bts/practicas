# practicas
//ejercicios
/*Necesitamos llevar un registro del stock de productos.
El cliente quiere saber el costo total de un pedido sumando el precio unitario por la cantidad de productos.
Requerimos solicitar datos al cliente para personalizar la experiencia.
Debemos verificar si tenemos suficiente stock para cubrir una demanda específica.
Hay que procesar una lista de productos pendientes de revisión. Primero intentaremos una solución con while y luego notaremos que for podría ser más elegante.
Condicionales:
Suponé que si el cliente quiere más de 100 unidades, le ofrecemos un descuento.
Implementá un if que verifique si cantidad > 100. Si es así, mostrá un mensaje indicando que aplica un descuento especial.
Bucles:
Pedile al usuario que ingrese un número, y luego usá un bucle for para imprimir desde 1 hasta ese número.
Repetí lo mismo con un while y compará cuál te resulta más intuitivo.
*/

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
      Scanner scanner = new Scanner(System.in);
      
      System.out.println("ingrese su nombre:  ");
      String nombre = scanner.next();
      System.out.println(nombre);
      System.out.println("ingrese cantidad: ");
      int cantidad = scanner.nextInt();
      System.out.println(cantidad);
      
      double costProduct = 4500;
      double costTotal = costProduct * cantidad;
      System.out.println("costo: " + costTotal);
      
      if (cantidad > 100) {
        System.out.println("hay descuento");
      } 
      
      System.out.println("ingrese un numero: ");
      int number = scanner.nextInt();
      
      for(int i=1; i <= number; i++) {
        System.out.println(i);
      } else {
        System.out.println("no aplica descuento");
      }
      
      int b = 1;
      while(b <= number) {
        System.out.println(b);
        b++;
      }
      
      scanner.close();
      
      
  }
}
