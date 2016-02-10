# SimpleCalculator

![jcinsanity](Screenshot 001l.PNG)

~~~
package ph.edu.dlsu;
import java.io.*;

public class Main {

    public static void main(String[] args) {
        String s1 = getInput("Input a number: ");
        String s2 = getInput("Input a number: ");

        double d1 = Double.parseDouble(s1);
        double d2 = Double.parseDouble(s2);
        double sum = d1 + d2;
        double mult = d1 * d2;

        System.out.println("The answer is(Sum): " + sum);
        System.out.println("The answer is(Mult): " + mult);
    }

    private static String getInput(String prompt) {
        BufferedReader stdin = new BufferedReader(
                new InputStreamReader(System.in));

            System.out.print(prompt);
            System.out.flush();

                try {
                    return stdin.readLine();
                } catch (Exception e){
                    return "Error:" + e.getMessage();
                }
        }
    }
    
~~~
