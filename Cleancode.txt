import java.lang.*;

import java.util.*;

class Cleancode 

{
    
	public static double principle1;

    	public static double time1;

    	public static double rateOfInterest1;
	public static double CompoundInterestvalue( double principle,double time,double rateOfInterest)
	{
        
		return principle*Math.pow(1.0+rateOfInterest/100.0,time) - principle;
    
	}
	public static double SimpleInterest( double principle,double time,double rateOfInterest)
    
	{
        
		return (principle*time*rateOfInterest)/100;
    
	}
	public static void main(String args[])
	{
        
	Scanner scan=new Scanner(System.in);
        
	principle1=scan.nextDouble();
        
	time1=scan.nextDouble();
        
	rateOfInterest1=scan.nextDouble();
        
	System.out.println(CompoundInterestvalue(principle1,time1,rateOfInterest1));
        
	System.out.println(SimpleInterest(principle1,time1,rateOfInterest1));
        
    
	}
}