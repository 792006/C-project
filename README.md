import java.util.Scanner;
class Operation{
    private long a,b,c;
    public Operation(){
        Scanner obj = new Scanner(System.in);
        System.out.println("Enter the First Number:");
        a=obj.nextInt();
        System.out.println("Enter the Second Number:");
        b=obj.nextInt();
    }
    public void disp(){
        System.out.println("Given Two Numbers are : "+a+" and "+b);
    }
    public void sum(){
        c= a+b;
        System.out.println("Sum of Given Two Numbers is "+c);
    }
    public void sub(){
        c= a-b;
        System.out.println("Sum of Given Two Numbers is "+c);
    }
    public void power(){
        System.out.println("Solution is "+Math.pow(a,b));
    }
    public void equality(){
        if(a==b){
            System.out.println("Both numbers are equal.");
        }
        else{
            System.out.println("Not Equal.");
        }
    }
    
    public void min(){
        if(a<b){
            System.out.println(a+" is less than "+b);
        }
        else{
            System.out.println(b+" is less than "+a);
        }
    }
    public void max(){
        if(a>b){
            System.out.println(a+" is greater than "+b);
        }
        else{
            System.out.println(b+" is greater than "+a);
        }
    }
    
    public void swap(){
        System.out.println("Numbers After Swapping are a="+a+" and b="+b);
        long temp=a;
        a=b;
        b=temp;
        System.out.println("Numbers After Swapping are a="+a+" and b="+b);
    }
    
}
public class Main {
    public static void main(String[] args){
        Operation a1 = new Operation();
        Scanner ob2 = new Scanner(System.in);
        
        System.out.println("Operations You Can Perform are:");
        System.out.println("1. Display Given Numbers");
        System.out.println("2. Addition of Given Numbers");
        System.out.println("3. Subtraction of Given Numbers");
        System.out.println("4. Power of a Number (first)^secondnum");
        System.out.println("5. Checking Equality of Two Numbers");
        System.out.println("6. Minimum of Two Numbers");
        System.out.println("7. Maximum of Two Numbers");
        System.out.println("8. Swap Two Numbers");
        
        
        int btn;
        System.out.println("Enter the number of Operation You have to Perform:");
        btn=ob2.nextInt();
        if(btn == 1){
            a1.disp();
        }
        else if(btn == 2){
            a1.sum();
        }
        else if(btn==3){
            a1.sub();
        }
        else if(btn==4){
            a1.power();
        }
        else if(btn==5){
            a1.equality();
        }
        else if(btn==6){
            a1.min();
        }
        else if(btn==7){
            a1.max();
        }
        else if(btn==8){
            a1.swap();
        }
    }
}
