package javaapplication2;

import java.util.Scanner;

public class JavaApplication2 {

    public static void main(String[] args) {
        Scanner captura = new Scanner(System.in);
        int edad;
        String genero;

        System.out.println("Digite su genero"
                + "\n M-Masculino "
                + "\n F-femenino "
                + "\n O-Otro ");

        genero = Leer.next();
        if (genero.equals("M")) {
            System.out.println("Digite su edad");
            edad = captura.nextInt();
            if (edad >= 18) {
                System.out.println("Bienvenido al ejercito nacional");
            } else {
                System.out.println("Usted no cuenta con la edad necesaria");
            }

        } else {
            System.out.println("Usted no es apto");
        }

    }

}

