# OddEvenSUmPositions
import java.util.Scanner;

public class OddEvenSUmPositions {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int NumbersCount = Integer.parseInt(scanner.nextLine());

        double OddSum = 0;
        double EvenSum = 0;
        double OddMin = Integer.MAX_VALUE;
        double OddMax = Integer.MIN_VALUE;;
        double EvenMin = Integer.MAX_VALUE;;
        double EvenMax = Integer.MIN_VALUE;;

        for (int i = 1; i <= NumbersCount; i++) {
            if (!(i % 2 ==0)){
                double NewOddNumber = Double.parseDouble(scanner.nextLine());

                OddSum += NewOddNumber;

                if (NewOddNumber > OddMax){
                    OddMax = NewOddNumber;
                }
                if (NewOddNumber < OddMin){
                    OddMin = NewOddNumber;
                }
            }
            else {
                double NewEvenNumber = Double.parseDouble(scanner.nextLine());

                EvenSum += NewEvenNumber;

                if (NewEvenNumber > EvenMax){
                    EvenMax = NewEvenNumber;
                }
                if (NewEvenNumber < EvenMin){
                    EvenMin = NewEvenNumber;
                }
            }
        }


        if (NumbersCount < 1){
            System.out.printf("OddSum =%.2f\n",OddSum);
            System.out.println("OddMin =No" );
            System.out.println("OddMax =No" );
            System.out.printf("EvenSum =%.2f\n",EvenSum);
            System.out.println("EvenMin =No" );
            System.out.println("EvenMax =No" );
        }
        else if (NumbersCount == 1){
            System.out.printf("OddSum =%.2f%n",OddSum);
            System.out.printf("OddMin =%.2f%n",OddMin);
            System.out.printf("OddMax =%.2f%n",OddMax);
            System.out.printf("EvenSum =%.2f%n",EvenSum);
            System.out.println("EvenMin =No" );
            System.out.println("EvenMax =No" );
        }
        else {
            System.out.printf("OddSum =%.2f%n",OddSum);
            System.out.printf("OddMin =%.2f%n",OddMin);
            System.out.printf("OddMax =%.2f%n",OddMax);
            System.out.printf("EvenSum =%.2f%n",EvenSum);
            System.out.printf("EvenMin =%.2f%n",EvenMin);
            System.out.printf("EvenMax =%.2f%n",EvenMax);
        }

    }
}
