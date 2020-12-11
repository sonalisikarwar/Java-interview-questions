# Java-interview-questions

class Factorial{
    //this is a recursive method 
    int fact(int n)  
    {
        int result;
        if(n==1) return 1;
        result = fact (n-1)*n;
        return result;
        }
}
class Recursion {
    public static void main(String args[]){
        Factorial f = new Factorial();
        System.out.println("Factorial of 3 is " +f.fact(3));
        System.out.println("Factorial of 3 is " +f.fact(4));
        System.out.println("Factorial of 3 is " +f.fact(5));
    }
    
}


//recursion
class RecTest{
    int values[];

    RecTest (int i ) 
    {
    values = new int[i];
    }
   
   void printArray(int i){
        if(i==0) return;
        else printArray(i-1);
        System.out.println("[" + (i-1) +"]"+ values [i-1]);
            }
        
    }
public class Recursion2 {
    public static void main(String args[]){
        RecTest ob = new RecTest(10);
        int i;
        
        for(i=0; i<10; i++ ) ob.values[i]=i;
        ob.printArray(10);
    }
    
}
