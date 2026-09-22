import java.util.Scanner;
 class ElectricityBill
{
  public static void main(String[] args)
{
  Scanner sc = new Scanner(System.in);
  int consumerNo;
  String consumerName;
  int prevReading, curReading;
  int conType;
  int units;
  double amount = 0;
  System.out.print("Enter Consumer Number: ");
  consumerNo = sc.nextInt();
  sc.nextLine();
  System.out.print("Enter Consumer Name: ");
  consumerName = sc.nextLine();
  System.out.print("Enter Previous Month Reading: ");
  prevReading = sc.nextInt();
  System.out.print("Enter Current Month Reading: ");
  curReading = sc.nextInt();
  System.out.println("\nSelect Connection Type");
  System.out.println("1. Domestic");
  System.out.println("2. Commercial");
  System.out.print("Enter your Choice: ");
  conType = sc.nextInt();
  units = curReading - prevReading;
   if(conType == 1)
     {
       if(units <= 100)
          amount = 0;
       else if(units <= 200)
          amount = (units - 100) * 2;
       else if(units <= 500)
          amount = 100 * 2 + (units - 200) * 4;
       else
          amount = 100 * 2 + 300 * 4 + (units - 500) * 6;
        }
    else if(conType == 2)
      {
         if(units <= 100)
           amount = units * 2;
         else if(units <= 200)
           amount = 100 * 2 + (units - 100) * 4;
         else if(units <= 500)
           amount = 100 * 2 + 100 * 4 + (units - 200) * 6;
         else
           amount = 100 * 2 + 100 * 4 + 300 * 6 + (units - 500) * 7;
        }
     else
      {
         System.out.println("Invalid Connection Type");
       }      
System.out.println("\nElectricity Bill");
System.out.println("Consumer Number : " + consumerNo);
System.out.println("Consumer Name   : " + consumerName);
if(conType == 1)
   System.out.println("Connection Type : Domestic");
else
   System.out.println("Connection Type : Commercial");
System.out.println("Units Consumed  : " + units);
System.out.println("Bill Amount     : Rs. " + amount);
    }
}
