# Java-program-to-find-the-power

## AIM:
To write a java program to find the power of a number raised to the other.

## PROCEDURE:
1. Import the necessary package: Start by importing the java.util.Scanner package, which allows user input from the console.
2. Define a public class named "Power" to encapsulate the program.
3. Define a main method inside it create an object for the Scanner.
4. Prompt the user for input, display the message "Enter the base:" and then use sc.nextInt() to read the user's input for the base and exponent and assign it to the base variable and exponent variable respectively.
5. Create a variable named re and assign it the value returned by calling the powerof method, passing the base and exponent as arguments.
6. Display the result, the message "Result: " followed by the value of re.
7. Outside the main method, define the public static int powerof(int a, int b) method, which takes two integers a and b as parameters and returns an integer.
8. Inside the powerof method, create an integer variable named result and initialize it to 1.
9. Calculate the power: Use a while loop to iterate while b is not equal to 0. Multiply result by a and decrement b by 1 in each iteration.
10. Return the result: After the while loop, return the value of result.
## PROGRAM:
```
import java.util.Scanner;

public class Power {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the base:");
        int base = sc.nextInt();
        System.out.println("Enter the exponent:");
        int exponent = sc.nextInt();

        int re = powerof(base, exponent);

        System.out.println("Result: " + re);
    }

    public static int powerof(int a, int b)
    {
        int result=1;
        while (b != 0)
        {
            result = result* a;
            --b;
        }
        return result;
    }

}
```

## OUTPUT:
```
C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=13490:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\java full stack\out\production\java full stack" Power
Enter the base:
2
Enter the exponent:
3
Result: 8

Process finished with exit code 0
```
## RESULT:
Thus, the java program to find the power of a number raised to the other is created and verified.
