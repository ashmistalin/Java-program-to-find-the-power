# Java-program-to-find-the-power

## AIM:
To write a java program to find the power of a number raised to the other.

## PROCEDURE:


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
