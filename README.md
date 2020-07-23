# matrix_multiplication_with_input
//Умножение двух матриц (с заданным размером). Элементы матрицы вводятся с клавиатуры 


package org.apache.poi.hssf.usermodel;

import java.sql.SQLOutput;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        int ni = 3;
        int nj = 5;

        int arr1[][] = new int[ni][nj];

        Scanner scanner = new Scanner(System.in);

        System.out.println("Input elements of array1: ");
        for (int i=0; i<ni; i++) {
            for (int j=0; j<nj; j++){
                arr1[i][j]=scanner.nextInt();
            }
        }


        int arr2[][] = new int[ni][nj];

        System.out.println("Input elements of array2: ");
        for (int i=0; i<ni; i++) {
            for (int j=0; j<nj; j++){
                arr2[i][j]=scanner.nextInt();
            }
        }


        for (int i = 0; i < ni; i++) {
            System.out.println();
            for (int j = 0; j < nj; j++) {
                System.out.print(arr1[i][j] + " " );
            }
        }
        System.out.println();
        System.out.println("------------------------");


        for (int i=0; i<ni; i++){
            System.out.println();
            for(int j=0; j<nj; j++){
                System.out.print(arr2[i][j]+ " " );
            }
        }

        System.out.println();
        System.out.println("------------------------");
        System.out.println("Новая перемноженная матрица");

        for (int i=0; i<ni; i++) {
            System.out.println();
            for(int j=0; j<nj; j++) {
                System.out.print(arr1[i][j] * arr2[i][j] + " ");
            }
        }

    }
}
