# Tutorial 6 - Answers

## Question 1

### Part A
public static int max(int a, int b, int c) {
    int max = a;
    if (b > max) max = b;
    if (c > max) max = c;
    return max;
}

### Part B
public static boolean isSquare(int num) {
    if (num < 0) return false;
    int root = (int) Math.sqrt(num);
    return root * root == num;
}

### Part C
public static long combination(int n, int k) {
    if (k < 0 || k > n) return 0;
    long result = 1;
    for (int i = 1; i <= k; i++) {
        result = result * (n - k + i) / i;
    }
    return result;
}

### Part D
public static boolean isPentagonal(int num) {
    int n = 1;
    int p = 1;                      // P1 = 1
    while (p < num) {
        n++;
        p = n * (3 * n - 1) / 2;
    }
    return p == num;
}

### Part E
public static void countLettersDigits(String s) {
    int letters = 0, digits = 0;
    for (int i = 0; i < s.length(); i++) {
        char ch = s.charAt(i);
        if (Character.isLetter(ch)) letters++;
        else if (Character.isDigit(ch)) digits++;
    }
    System.out.println("Letters: " + letters);
    System.out.println("Digits: " + digits);
}

### Part F
public static void generateRandoms(int[] numbers) {
    Random rand = new Random();
    for (int i = 0; i < 10; i++) {
        numbers[i] = rand.nextInt(101);   // 0 to 100
    }
}

### Part G
public static void circle(double radius, double[] result) {
    result[0] = Math.PI * radius * radius;   // area
    result[1] = 2 * Math.PI * radius;        // circumference
}

### Part H
public static int firstRepeated() {
    Random rand = new Random();
    boolean[] seen = new boolean[11];
    while (true) {
        int num = rand.nextInt(11);   // 0 to 10
        if (seen[num]) return num;
        seen[num] = true;
    }
}

## Question 2

public class DecreasingOrder {

    public static void displayDecreasing(int a, int b, int c) {
        int temp;

        if (a < b) { temp = a; a = b; b = temp; }   // now a >= b
        if (a < c) { temp = a; a = c; c = temp; }   // now a is the largest
        if (b < c) { temp = b; b = c; c = temp; }   // now b >= c

        System.out.println(a + " " + b + " " + c);
    }

    public static void main(String[] args) {
        displayDecreasing(4, 9, 2);    // 9 4 2
        displayDecreasing(10, 3, 7);   // 10 7 3
        displayDecreasing(5, 5, 1);    // 5 5 1
    }
}
