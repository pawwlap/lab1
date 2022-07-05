# lab1
package pl.lublin.wsei.java.wykl2;
import pl.lublin.wsei.java.wykl2.mylib.Account;

import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
    int a = 5;
    double b = 7.56;
    String s = "jakis tekst";
    System.out.printf("a = %d, b = %.2f, s = %20s \n",a,b,s);

    System.out.println("alfa\tsin(alfa)\n");
    for (int i = 0; i <370; i+=10)
        System.out.printf("%d\t%f\t\n", i, Math.sin(i/360.0*3*Math.PI));

    Scanner input = new Scanner(System.in);
    int num1=0, num2=0;
    do {
        System.out.print("podaj pierqwsza liczbe :");
        num1= input.nextInt();
        if (num1 !=0)
        {
            System.out.print("podaj druga liczbe: ");
            num2 = input.nextInt();
        }
    }while ((num1 != 0) && (num2 != 0) );

        Account acc = new Account();
        acc.setName("Piotr Gołabek");
        System.out.println(acc.getName());

    }
}
