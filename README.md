# TASKK 1
package ass1;
import java.util.Scanner;
public class guessingnumber {
    public static void
    guessingnumbergame()
    {
    	Scanner sc= new Scanner(System.in);
    	int number=1+(int) (100*Math.random())	;
    	
    	int k=5;
    	int i,guess;
    	System.out.println("Guess a number between 1 to 100 within"+ k+ "trials");
    	for(i=0;i<k;i++) {
    		System.out.println("Guess the number");
    	guess=sc.nextInt();
    	if(number==guess) {
    		System.out.println("Congrats, your guess is correct");
    		break;
        }
    	else  if(number<guess && i!=k-1){
    	 System.out.println("Your guess is too high");
        }
    	else if(number>guess && i!=k-1){
    	 System.out.println("Your guess is too low");
    	}
    	}

    if(k==i)
	   System.out.println("You have exhausted your total no of trials");
       System.out.println("The number was"+ number);
    }


	public static void main(String[] args) {
		guessingnumbergame();

	}

	}
