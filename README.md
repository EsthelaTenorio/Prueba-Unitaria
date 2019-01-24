# Prueba-Unitaria

import java.util.Scanner;

/**
 *
 * @author DELL
 */
public class Pry_Pruebas_Unitarias {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
             OperacionesP op=new OperacionesP();
       Scanner teclado=new Scanner(System.in);
       
        float num1,num2, result=0;
        int opciones;
        do{
        System.out.println("\t PROGRMA DE PRUEBAS UNITARIAS");
        System.out.println("1.SUMA");
        System.out.println("2.RESTA");
        System.out.println("3. MULTIPLICACION");
        System.out.println("4. DIVISION");
        
        System.out.println("\t ELIJA LA OPCION PORFAVOR");
        
        opciones=teclado.nextInt();
        
        System.out.print("Ingrese el primer numero:");
        num1=teclado.nextFloat();
        System.out.print("Ingrese el segundo numero:");
        num2=teclado.nextFloat();
   
        switch(opciones){
            case 1:
                result=op.Suma(num1,num2);
                //System.out.println("La suma es:"+resul);
            break;
            case 2:
                result=op.Restar(num1, num2);
                //System.out.println("La resta es:"+resul);
            break;
            case 3:
                result=op.Multiplicar(num1, num2);
                //System.out.println("La multiplicacion es:"+resul);
            break;
            case 4:
                result=op.Dividir(num1, num2);
                //System.out.println("La division es:"+resul);
            break;
                
        }    
    }while(opciones!=4);
    }
    }
Operaciones Basicas
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package pry_pruebas_unitarias;

/**
 *
 * @author DELL
 */
public class OperacionesP {
     float num1;
     float num2;
     float result;
    public float Suma(float num1,float num2){
        result=(float) (num1+num2);
        System.out.println("LA SUMA ES:"+result);
        return result;
    }
    public float Restar(float num1,float num2){
        result=(float) (num1-num2);
         System.out.println("LA RESTA ES:"+result);
        return result;
    }
    public float Multiplicar(float num1,float num2){
        
        result=(float) (num1*num2);
         System.out.println("LA MULTIPLICACION ES:"+result);
        return result;
    }
    public float Dividir(float num1,float num2){
        
        result=(float) (num1/num2);
         System.out.println("LA LA DIVISION ES:"+result);
        return result;
    }
}
