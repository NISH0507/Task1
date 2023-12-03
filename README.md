# Task1
import java.util.Random;
public class NumberGame {
    Random re=new Random();
    double   generatedNo= re.nextInt(100)+1;
    {

        System.out.println("generated no is:"+generatedNo);
    }


}
import java.util.Scanner;
public class MainApp1 {
    public static void main(String[] args) {
        Scanner sc1 = new Scanner(System.in);
        NumberGame n1= new NumberGame();

        while (true){
            System.out.println("enter your guessno");
            double guessno = sc1.nextDouble();
            if(guessno== n1.generatedNo){
                System.out.println("no is matched");
                break;
            }
            else if(guessno< n1.generatedNo){
                System.out.println("no is lower then generated no");

            }
            else{
                System.out.println("no is higher then generated no");
            }

        }
