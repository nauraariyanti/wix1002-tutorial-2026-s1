# Tutorial 02 — Answers

### Question 1

a. public class Display {
    public static void main(String[] args) {
        System.out.print("Faculty of ");
        System.out.print("Computer Science ");
        System.out.print("and ");
        System.out.println("Information Technology.");
    }
}

b. public class Display {
    public static void main(String[] args) {
        System.out.println("Faculty of\nComputer Science\nand\nInformation Technology.");
    }
}


### Question 2

System.out.println("\"SDN\" - Software-defined networking");


### Question 3

Correct the error for the following statements.
a. System.out.println("Java Programming");
b. System.out.println("Introduction to Java!")
c. System.out.println("\\t is the horizontal tab character");
d. System.out.println("Java is case sensitive!" );

### Question 4

int matricNumber;
double pi;
Boolean M = false;
long P = 8800000000L;
char P = 'U';
final String PRO = "Java";

### Question 5

a.
double amount = 32.5;
AMOUNT += 10;
System.out.println("The amount is " + amount);

b.
String chapter = "Summary";
System.out.println(chapter);

c.
int num = 0;
num++;
num1 = num;

d.
double num = 3000;
System.out.printf("%4.2f\n", num);

e.
import java.util.Scanner;

String contact;
Scanner keyboard = new Scanner(System.in);
contact = keyboard.nextLine();

### Question 6

import java.util.Scanner;

public class CircleCircumference {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter the diameter of the circle: ");
        double diameter = input.nextDouble();

        double circumference = Math.PI * diameter;

        System.out.printf("The circumference of the circle is %.3f\n", circumference);

        input.close();
    }
}

### Question 7

import java.util.Scanner;

public class InchesToMeters {
    public static void main(String[] args) {
        final double CM_PER_INCH = 2.54;
        final double CM_PER_METER = 100;

        Scanner input = new Scanner(System.in);

        System.out.print("Enter the length in inches: ");
        double inches = input.nextDouble();

        double centimeters = inches * CM_PER_INCH;
        double meters = centimeters / CM_PER_METER;

        System.out.printf("%.2f inches is equal to %.2f meters\n", inches, meters);

        input.close();
    }
}
