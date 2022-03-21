# home-work-1

1. (a) Create a class PayCalculator that has an attribute payRate given in
dollars per hour. The class should also have a method computePay(hours)
that returns the pay for a given amount of time.

import java.math.BigDecimal;
public abstract class PayCalculator {
		BigDecimal payRate;
		public PayCalculator(BigDecimal payRate){
			this.payRate = payRate;
		}
		public abstract BigDecimal computePay(float hour); 

	Import java.math.BigDecimal;
	Public class RegularPay extends PayCalculator {
		Public RegularPay(BigDecimal payRate){
			Super(payRate);
		}
		Public BigDecimal computerPay(float hour){
			Return (payRate.multiply(new BigDecimal(hour));
		}
	}
	Import java.math.BigDecimal;
	Public class HazardPay extends PayCalculator {
		Public HazardPay(BigDecimal payRate){
			Super(payRate);
		}
		Public BigDecimal computerPay(float hour){
Return payRate.multiply(new BigDecimal(hour)).multiply(new BigDecimal(1.5));
		}
	}

(b) Derive a class RegularPay from PayCalculator, as described in 1(a) above exercise. 
It should have a constructor that has a parameter for the pay rate. It should not override any of the methods. Then derive a class HazardPay from PayCalculator that overrides the computePay method. The new method should return the amount returned by the base class method multiplied by 1.5.
( Copy the code here)
import java.math.BigDecimal;
public class HomeworkOne {
	public static void main(String [] args) {
		BigDecimal payRate = new BigDecimal(35);
		RegularPay rp = new RegularPay(payRate);
		System.out.println(rp.computePay(10));
		
		PayCalculator pay = new HazardPay(payRate);
		System.out.println(pay.computePay(10));
	}

}
Copy results screen shot here: 
2. Write a program that lets the user guess whether the flip of
a coin results in heads or tails. The program randomly generates an integer 0 or 1,
which represents head or tail. The program prompts the user to enter a guess and
reports whether the guess is correct or incorrect.
Use following to rendomly generate 0 or 1
   // Obtain the random number 0 or 1
    int number = (int)(Math.random() * 2);
(Copy the program and its output here)
import java.util.Scanner;
import java.util.Random;
public class Homework1TailHead {
		  public static void main(String[] args){
		        @SuppressWarnings("resource")
				Scanner in = new Scanner(System.in);
		        Random random = new Random();
		        int coin_flip = random.nextInt(2);
		        System.out.print("Enter 1 for heads, 0 for tails CoinFlip ");
		        int guess = in.nextInt();
		        if(guess == coin_flip){
		            System.out.println("You guess right, congrats!");
		        }else{
		            System.out.println("Sorry, you guessed wrong, try again.");
		        }


		
	}

}
( Copy the result screen shot😊
 
3.Which of the following assignment statements is correct to assign character 5 to c?
	
a. 	char c = 5;
b. 	char c = “5";
c. 	char c = '5';
d. 	char c = "344";
	b. 	char c = “5";
4. What is the output of the following code: (Please indent the statement correctly first.)
int x = 9;
int y = 8;
int z = 7;    
if (x > 9)
    if (y > 8)
        System.out.println("x > 9 and y > 8");
else if (z >= 7)
    System.out.println("x <= 9 and z >= 7");
else 
    System.out.println("x <= 9 and z < 7");
a. 	x > 9 and y > 8;
b. 	x <= 9 and z >= 7;
c. 	none
d. 	x <= 9 and z < 7;
  
	c. 	none


