package Pricipal;
import Logica.ListasEnlazada;
import java.util.Scanner;

public class Main {
    public static void main(String args[]){
        Scanner leer = new Scanner(System.in);
        ListasEnlazada  obj = new ListasEnlazada ();
       boolean continuar = true;
               String insertar;
       int  menu=0;
    
        while(continuar){
    
        System.out.println("BIENVENIDOS AL MENU DE LISTAS ENLAZADAS \n"
                   + "1: INSERTAR AL INICIO\n"
                   + "2: INSERTAR EN ALGUNA POSICION \n"
                   + "3: INSERTAR AL FINAL \n"
                   + "4: ELIMINAR"+"\n"
                   + "5: MOSTRAR "+"\n"
                   + "6: SALIR");
        menu=leer.nextInt();
        
          switch(menu){
              case 1:
                  System.out.println(" Palabra a insertar");
                insertar=leer.next();
                obj.InsertarAlInicio(insertar);
                break;
            case 2:  
               System.out.println(" Palabra a insertar");
                insertar=leer.next();
                obj.InsertarPosicion(insertar);
               break;
            case 3:
                 System.out.println(" Palabra a insertar");
                insertar=leer.next();
                obj.InsertarAlfinal(insertar);
                break;
            case 4:
                obj.eliminar();
                break;
                case 5:
                obj.mostrar();
                break;
                case 6:
                    System.out.println("fuera");
                    continuar =false;
                break;
                 default:
                 System.out.println("opcion incorrecta");
                 break;
           
          }
     }
  }
}
