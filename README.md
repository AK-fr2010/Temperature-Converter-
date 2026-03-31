# Temperature-Converter-

    import java.util.Scanner;
     public class Main {
      public static void main(String[] args){
        Scanner scanner = new Scanner(System.in);

        double temp ;
        double newTemp ;
        String unit ;

        System.out.println("---------------------------");
        System.out.println("Temperature Converter v1.0");
        System.out.println("---------------------------");

        System.out.print("Please Enter The Temperature : ");
        temp = scanner.nextDouble();

        System.out.print("Please Enter to which unit you want to convert it into -> Celsius or Fahrenheit ( C or F ) : ");
        unit = scanner.next().toUpperCase();

        newTemp = (unit.equals("C")) ? (temp - 32) * 5 / 9 : (temp * 9 / 5) + 32 ;

        System.out.printf("The New Temperature is %.2f" , newTemp);

        scanner.close();
    }
}
