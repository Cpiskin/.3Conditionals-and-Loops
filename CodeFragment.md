Write a program code fragment that puts the binary representation of a positive integer n into a String variable s.

int n = 42; // Replace with the positive integer you want to convert
String s = "0"; // Initialize the string with "0"

while (n > 0) {
    int remainder = n % 2;
    s = remainder + s; // Prepend the remainder to the string
    n = n / 2;
}

System.out.println("Binary representation: " + s);
