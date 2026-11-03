# Tutorial 03 - Answers

## Question 1

### Part A

boolean isEqual = (3*8 == 27);

### Part B

if (number % 2 == 0) {
    System.out.println("Even");
} else {
    System.out.println("Odd");
}

### Part C

boolean isUpper = (ch >= 'A' && ch <= 'Z');

### Part D

if (s1.compareToIgnoreCase(s2) <= 0)
    System.out.println(s1 + " " + s2);
else
    System.out.println(s2 + " " + s1);

### Part E

int day = scanner.nextInt();

switch (day) {
    case 0: System.out.println("Sunday");    break;
    case 1: System.out.println("Monday");    break;
    case 2: System.out.println("Tuesday");   break;
    case 3: System.out.println("Wednesday"); break;
    case 4: System.out.println("Thursday");  break;
    case 5: System.out.println("Friday");    break;
    case 6: System.out.println("Saturday");  break;
    default: System.out.println("Invalid input");
}

## Question 2

### Part A
if (num1 == num2) 
System.out.println("Number 1 is equal to number 2.");


### Part B
if (x > y && y > z)
 System.out.println("x is the largest number");

### Part C
String s1 = "hello", s2 = "hello";

if (s1.equals(s2))
 System.out.println("They are equal strings.");
else 
 System.out.println("They are not equal strings.");

### Part D
if (x>0 || y>0);
 System.out.println("Either x or y is positive");

## Question 3

### Part A
#####
$$$$$

### Part B
#####
$$$$$

### Part C
#####

### Part D
nothing is printed

## Question 4

Scanner input = new Scanner(System.in);
System.out.print("Enter three integers: ");
int a = input.nextInt();
int b = input.nextInt();
int c = input.nextInt();

if (a >= b && a >= c)
    System.out.println("The biggest number is " + a);
else if (b >= a && b >= c)
    System.out.println("The biggest number is " + b);
else
    System.out.println("The biggest number is " + c);


## Question 5

Scanner input = new Scanner(System.in);
System.out.print("Enter a year: ");
int year = input.nextInt();

if ((year % 4 == 0 && year % 100 != 0) || year % 400 == 0)
    System.out.println(year + " is a leap year");
else
    System.out.println(year + " is not a leap year");
 
