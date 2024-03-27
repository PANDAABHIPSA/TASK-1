# TASK-1

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
	   System.out.pr…

import java.util.Scanner;
public class gradecalculator {

	public static void main(String[] args) {
int marks[]= new int[6];
int i, total=0, avg;
Scanner sc= new Scanner(System.in);

for(i=1;i<6;i++) {
	System.out.println("Enter the mark of subject"+ i );
	marks[i]=sc.nextInt();
	total= marks[i]+ total;
}
avg=total/i;
System.out.println("Grade of the student is:");
if(avg>=80)
{
    System.out.print("A");
}
else if(avg>=60 && avg<80)
{
   System.out.print("B");
} 
else if(avg>=40 && avg<60)
{
    System.out.print("C");
}
else
{
    System.out.print("D");
}
System.out.println("Total marks secured is"+ total);
System.out.println("Average is "+ total/5);
System.out.println("Average% is "+ (avg/5)*100);
}
	
}
