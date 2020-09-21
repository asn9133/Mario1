package com.company;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        int height;
        do{
            System.out.println("Enter the height of the pyramid");
            height = input.nextInt();
        }while(height <1 || height >8);

        int i,j,k;

        //rows
        for(i=0; i<height; i++){
            //spaces
            for(j=height-1; j>i; j--){
                System.out.print(" ");
            }
            //columns
            for(k=-1; k<i; k++){
                System.out.print("#");
            }
            System.out.println();
        }
    }
}
