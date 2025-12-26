# ganesh-demo
This is my first Git Repository
package cse;

import java.util.Random;
import java.util.Scanner;

public class RandomNumberGenerator
{

	public static void main(String[] args) 
	{
		Scanner scanner = new Scanner(System.in);
		Random random = new Random();
		
		int randomNumber = random.nextInt(100)+1;
		int guess = 0;
		int attempts = 0;
		
		System.out.println("Welcome to the RandomNumberNumber Guessing Game!");
		System.out.println("I have selected a number between 1 and 100 . Try to guess it!");
		while ( guess != randomNumber)
		{
			System.err.println("Enter your guess:");
			guess = scanner.nextInt();
			attempts++;
			
			if (guess < randomNumber)
			{
				System.out.println("Too low! Try again.");				
			}
			
			else if (guess > randomNumber)
			{
				System.out.println("Too high! Try again.");
				
			}
			
}
		
		scanner.close();
	

	}

}
			else
			{

				System.out.println("Correct! The number was" + randomNumber+".");
				System.out.println("You guessed it in" + attempts + "attempts.");
				
			}
			
			
		