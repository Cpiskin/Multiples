// Import Scanner
import java.util.Scanner;

public class Multiples {
    public static void main(String args[]) {
      
      //Create a scanner object
      Scanner s = new Scanner(System.in);
      
      //Get the range
      System.out.println("Enter range ==> ");
      int num = s.nextInt();
      
      //Create 2 variables to calculate the sum
      int count = 0;
      int count2=0;
      
      //Create a for loop to get all the number until the range finishes
      for(int i=1; i<num; i++){
          //Check if i is disidible by 7 or 8
          if(i%7==0 || i%8==0){
              count += i;
          }
          //Check if i is divisible by 3 or 5
          if(i%3==0 || i%5==0){
              count2 += i;
          }
      }
      
      //Find the difference
      int dif = count - count2;
      //Get the absulute value of the difference
      int diff = Math.abs(dif);
      
      //Print all the values
      System.out.println("Multiple total of 3 and 5: "+count2);
      System.out.println("Multiple total of 7 and 8: "+ count);
      System.out.println("Difference "+ diff);
      
    }
}
