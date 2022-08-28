# parcial

package progra.Parcial_1;

import java.util.Scanner;
import progra.ArrayFunciones;

/**
 *
 * @author Julio Ramos
 */
public class Inicio {
    
  public static void main(String[] args) {

           boolean salir = false;
           int opcion; 
           
           Datos a = new Datos();

      
           Scanner sn = new Scanner(System.in);   
      
              do{
           System.out.println("Selecciona la informacion que desee llenar. ");
           System.out.println("1. Patient");
           System.out.println("2. Doctor");
           System.out.println("3. Nurse");
           
           System.out.println("Escriba el numero de una de las opciones");
           
           opcion = sn.nextInt();
           
           switch(opcion){
               case 1:
                   a.Patient();            
                   break;
               case 2:
                   a.Doctor();
                   break;
                case 3:
                   a.Nurse();
                   break;
                case 4:
                    System.out.println("Salio de la aplicacion.");
                    salir=true;
                   break;
                default:
                   System.out.println("Solo números entre 1 y 4");
            }
       }while(!salir);
}
  }
  
  ________________________________________________________________________________________
  
  
  public class Datos {
    
    public void Patient( )//Función sin parámetros
        {
           
        int id;
        String name = null;
        String email;
        String phoneNumber;
        
        
        Scanner sn = new Scanner(System.in); 
        System.out.println("Ingrese el nombre del paciente: ");
        System.out.print(name);
        
        }
      
    public void Doctor( )//Función sin parámetros
        {
           
        int id;
        String name;
        String email;
        String phoneNumber;
        }
            
     public void Nurse( )//Función sin parámetros
        {
           
        int id;
        String name;
        String email;
        String phoneNumber;
        }
      
}
