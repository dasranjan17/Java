/*Program to print the sum of negative numbers, sum of positive even numbers and the sum of positive odd numbers from a list of numbers (N) entered by the user. The list terminates when the user enters a zero*/

import java.util.*;
class allSum {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int sumN=0, sumO=0, sumE=0;
        int n;
        System.out.print("Enter the numbers: ");

        do {
            for(int i=1; ; i++){
                n=sc.nextInt();

                if (n<0){
                sumN=sumN+n;
                } else if(n>1 && n%2==0){
                sumE=sumE+n;
                } else if(n>0 && n%2!=0){
                sumO=sumO+n;
                } else{
                break;
                }
            } 
        } while(n!=0);

        System.out.println("The sum of negative numbers is "+sumN);
        System.out.println("The sum of postive even numbers is "+sumE);
        System.out.println("The sum of postive odd numbers is "+sumO);
    }
}

