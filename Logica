package Logica;

import CreadorNodo.Nodo;
import java.util.Scanner;

public class ListasEnlazada {
    
    Nodo raiz =null;
    Nodo cima= null;
    Nodo anterior =null;
    Nodo siguiente = null;
    int tamaño =0,posicion,contador=1;
    boolean repetir=true;
    Scanner leer = new Scanner(System.in);
    
    
    public void InsertarAlfinal(Object insertar){
        Nodo nodoactual = new Nodo(insertar);
         if(raiz==null){
         raiz=nodoactual;
         cima= nodoactual;
         }else{
         cima.siguiente=nodoactual;
         cima= nodoactual;
         }
         tamaño++;
    }
     public void InsertarAlInicio(Object insertar){
        Nodo nodoactual = new Nodo(insertar);
         if(raiz==null){
         raiz=nodoactual;
         cima= nodoactual;
         }else{
         nodoactual.siguiente=raiz;
         raiz=nodoactual;
         }
         tamaño++;
    }
     public  void InsertarPosicion(Object insertar){
     Nodo aux =raiz;
         System.out.println("auxiliar:"+aux.elemento);
         System.out.println("raiz:"+raiz.elemento);
         System.out.println("cima:"+cima.elemento);
         Nodo nodoactual = new Nodo(insertar);
         if(raiz==null){
         raiz=nodoactual;
         cima= nodoactual;
         }else{
         while(repetir){
             System.out.println("¿QUE POSICION DESEAS INSERAR?");
             posicion=leer.nextInt();
             if(posicion>tamaño){
             
                 System.out.println("solo puedes insertar hasta la posicion: "+(tamaño+1));
             }else {
             repetir=false;
             
             }
         }
         if(posicion==1){
         nodoactual.siguiente=raiz;
         raiz=nodoactual;
            } else{
             int i=1;
         for(i=1;i<= posicion;i++){
            
         if(i==posicion-1){
         anterior=aux;
         siguiente=aux.siguiente;
         }else{
         aux=aux.siguiente;
         }
        }
         cima=raiz;
          for(i=1;i<= tamaño;i++){
          if(cima.elemento.equals(anterior.elemento)){
          cima.siguiente=nodoactual;
          cima=nodoactual;
          nodoactual.siguiente=siguiente;
          }else{
          cima=cima.siguiente;
          }
        }
      }
   }
         tamaño++;
  }
     
     
     public void eliminar(){
     if(raiz==null){
         System.out.println("NO EXISTE NINGUN ELEMENTO A ELIMINAR");
     }else {
     raiz =raiz.siguiente;
     tamaño--;
         System.out.println("DATO ELIMINADO");
     }
  }
     
     public void mostrar(){
     Nodo auxiliar=raiz;
     if(auxiliar==null){
         System.out.println("NO EXISTE NINGUN ELEMENTO A MOSTRAR");
     }else{
     while(auxiliar!=null){
         System.out.println(" "+auxiliar.elemento);
         auxiliar=auxiliar.siguiente;
     }
   }
  }
}
