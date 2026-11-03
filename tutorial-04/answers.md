# Tutorial 04 - Answers

## Question 1

### Part A
int n = 1;

while ((n + 1) * (n + 1) * (n + 1) < 2000)
    n++;

System.out.println("The largest n is " + n);

### Part B
for (int i = 1; i <= 12; i++)
    System.out.println(i + " squared is " + (i * i));

### Part C
for (int row = 0; row < 4; row++) {
    for (int col = 0; col < 5; col++) {
        int value = (int) (Math.random() * 101);
        System.out.printf("%5d", value);
    }
    System.out.println();
}

### Part D
Scanner input = new Scanner(System.in);
System.out.print("Enter a number: ");
int number = input.nextInt();

int sum = 0;
for (int i = 1; i <= number; i++)
    sum += i;

System.out.println("The sum from 1 to " + number + " is " + sum);

### Part E
double sum = 0;

for (int i = 1; i <= 25; i++)
    sum += (double) i / (26 - i);

System.out.printf("The sum is %.2f%n", sum);

## Question 2

### Part A
int sum = 0;
for (int x = 10; x > 0; x--)
    sum += x;

### Part B
do {
 x += 2;
 y += x;
 System.out.println(x + " and " + y);
}
while (x < 100);

### Part C

for (int x=1, y=20; x < y; x++, y-=2);
 System.out.println(x + " " + y);

### Part D
int i = 1;
while (i<10) {
    i++;
}
System.out.println("Program End");

## Question 3

int f1 = 1, f2 = 1;

System.out.print(f1 + " " + f2);

for (int n = 3; n <= 10; n++) {
    int fn = f1 + f2;
    System.out.print(" " + fn);
    f1 = f2;
    f2 = fn;
}
System.out.println();

## Question 4

Scanner input = new Scanner(System.in);
System.out.print("Enter a string: ");
String str = input.nextLine();

for (int i = str.length() - 1; i >= 0; i--)
    System.out.print(str.charAt(i));
System.out.println();
