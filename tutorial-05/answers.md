# Tutorial 03 - Answers

## Question 1

### Part A
float[] numbers = new float[12];

### Part B
char[] letters = {'A', 'B', 'C', 'D', 'E'};

### Part C
String[] names = new String[100];

### Part D
int[][] table = new int[6][2];

### Part E
int[][] numbers = {
    {6, 9},
    {2, 5},
    {4, 6}
};

### Part F
numbers[1][1] = 4;
numbers[2][0] = 3;
numbers[2][1] = 7;

## Question 2

### Part A
String[] code = {"AAA", "AAB", "AAC", "AAD"};

### Part B
int[] num = new int[10];

int sum = 0;
for(int k=0; k<=num.length; k++)
  sum+=num[k];

### Part C
int[][] t = new int[3][3];
t[1][2] = 5;

### Part D
int i=4;
int []score = new int[5];
score [1] = 78;
score[i++] = 100;

## Question 3

marks[0] = 961;
marks[1] = 31;
marks[2] = 1;
marks[3] = 31;
marks[4] = 31;

## Question 4
int count = 0;

for (int i = 0; i < sentence.length; i++) {
    if (sentence[i].equals("the")) {
        count++;
    }
}

System.out.println("Number of occurrences of the: " + count);

## Question 5
for (int i = sentence.length - 1; i >= 0; i--) {
    for (int j = sentence[i].length() - 1; j >= 0; j--) {
        System.out.print(sentence[i].charAt(j));
    }
    System.out.println();
}

## Question 6
import java.util.Random;

public class Main {
    public static void main(String[] args) {

        Random rand = new Random();

        int num = rand.nextInt(256);

        int[] binary = new int[8];

        for (int i = 7; i >= 0; i--) {
            binary[i] = num % 2;
            num = num / 2;
        }

        for (int i = 0; i < 8; i++) {
            System.out.print(binary[i]);
        }
    }
}


