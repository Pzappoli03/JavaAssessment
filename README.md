# JavaAssessment1.	Create a class called MyClass, with a main method that prints your name. (5 points)
       
	   public class Name{
            public String fName;
            public String lName;

            public Name(){
            fName = "Pam";
            lName = "Zappoli";
    }

        public Name(String name1, String name2){
        fName = name1;
        lName = name2;
    }

        public void printName(){
                 System.out.println(fName+" "+lName);
    }
	
			 
2.	Create a class called MyClass, with a main method that prints in new lines the following array of values (5 points)
    a.	Apple, Orange, Pineapple, Banana, Berry, Peach
        
		public class MyClass {
           public static void main(String[] args) {
           String[] fruits = {"Apple", "Orange", "Pinapple", "Banana", "Berry", "Peach"};
           for (String tempFruits: Fruits) {
           System.out.println(tempFruits);

3. 	Create two classes: ClassA and ClassB. ClassA will contain the main method while ClassB has a method called identifyClass. (identifyClass returns no value)
        a.	Use instantiation to reach out to the identifyClass method (4 points)
		
		public class ClassA {
           static String identifyClass(){
           return "This is ClassA's method";
		
		public class ClassB {
            public static void main(String[] args){
            ClassA myClass = new ClassA();
            System.out.println(myClass.identifyClass(){
			}
			
		
        b.	Use inheritance to reach out to the identifyClass method (3 points)
        
		public class ClassC extends ClassA {
            public static void main(String[] args){
            System.out.println(identifyClass());
    }
	
4.  Create a method that returns back the largest number in an array of integers (5 points)
    a.The method should receive an array of integers


	
	
5.	Create a method that returns a random number from 1-100 (3 points)

    public class RandomNumber {
    public static void main(String[] args) {
        for(int i = 0; i < 10; i++) {
            randomNum(100);
        }
    }

    public static void randomNum(long range){
        System.out.println((long)(Math.random()*range));
    }

6.	Create a method that receives an integer argument from 0-100 and returns your test grade in a String format. (10 points)
    a.	Example: Input = 79	Output = “Your score of 79 got you a C.”
	
	public static void main(String[] args) {
    // This is step #1
    int score = 70;

    //This is step #2
    if (score >= 90) {
        System.out.println("Your grade is A...");

    } else if (score >= 80 && score <= 89) {
        System.out.println("Your grade is B...");

    } else if (score >= 70 && score <= 79) {
        System.out.println("Your grade is C...");

    } else if (score >= 60 && score <= 69) {
        System.out.println("Your grade is D...");

    }
    else {
        if (score >=0) {
         System.out.println("Your grade is F...");

        }
        else {
            System.out.println(score + " is an invalid score. Please use another score. ");

        }
    }

7.	Create a main method that loops through a double array of integers. The loop should output the value of the greatest number. (10 points)
    a.	Requirements: Row > 5 and Col > 5
    b.	Define your double array
	
    public class DoubleDimensionArray {
        static final int ROWS = 5;
        static final int COLS = 6;

    public static void main(String[] args) {
        String[][] matrixNumbers = {{"00","01","02","03","04"},
                {"14","15","16","17","18","19"},
                {"21","21","22","23","24","25"}};

        for (int row = 0; row <= 5; row++){
            for(int col = 0; col <= 6; col++){
                if(matrixNumbers[row][col] == "AA"){
                    System.out.print("Row = "+row);
                    System.out.print(" Col = "+col);
                    System.out.println("\nRow = "+row+" Col = "+col);
                }
            }
        }

	
	
8.	Create a method (no need for a main)
    
	public void printDivisibleBySix(int start, int stop){
	     for(int i=start; i <=stop; i++){
		     if(i%6 ==0){
		     System.out.println(i);
		 }
     
}		 
	       
    
	
9.	Create me a class called ClassA that contains 2 private double fields and a default constructor. The constructor should default the values to zero. Use encapsulation for both private fields. (10 points)
    
	public class ClassA {
    private double field1;
    private double field2;

    public ClassA(double num1, double num2){
        field1=num1;
        field2=num2;
    }

    public ClassA(){
        field1 = 0;
        field2 = 0;
    }

    public void sendMsg(){
        System.out.println("Num1 = "+field1+"\nNum2 = "+field2);
    }
}


10.	Create me an Interface that has one of each: 1 abstract method, 1 default method and 1 static method (10 points)
    a.	Requirements: Static method must be called from default method

	public interface InterA[
       String NAME = "My name is Pam...";

     default void identifyInterface(){
        System.out.println("This is interface A....");
        returnStaticMessage();
    }

    default void someOtherMethod(){
        returnStaticMessage();
    }

    default int letsDoSomething(){
        returnStaticMessage();
        return 1;
    }

        void returnMessage();

   
    static void returnStaticMessage(){
        System.out.println("This is your static method from the interface....");
    }
}
    

11.	Create me a class called ClassA that uses inheritance with ClassB and implements InferfaceA. (5 points)
    a.	Requirements: Add Constants to Interface (at least one)
    
	public class ClassA extends ClassB implements InterA{
    private String strMessage;

    public String getStrMessage() {
        return strMessage;
    }

    public void setStrMessage(String strMessage) {
        this.strMessage = strMessage;
    }

    public void identifyClasses(){
        System.out.println("This is Class A....");
    }
     // Identify Class B extension
    public void identifyOtherClasses(){
        identify(); 
    }

    public void returnMessage(){
        System.out.println("This is ClassA implementing an abstract method from InterfaceA....");

12.	Create a method that returns the division of two numbers. Implements try/catch for the ArithmeticException. (5 points)
   a.	Requirements: both numbers have to be passed as arguments
    
	    public double div(double num1, double num2){
        try {
            return num1 / num2;
        }catch(ArithmeticException ae){
            System.out.println("Can't divide by 0...");
        }
        return -1;
    }
}



13.	Create a class called ClassA with a main method. Create a second class called ClassB that contains a method called indentifyClass. ClassA calls for identifyClass. 
    If you do not wrap ClassB’s method with a try/catch how else can you catch the exception? Hint: be the lazy developer and the pro-active developer. (15 points)
    
	public class ClassA {
    public static void main(String[] args){
        ClassB aClass = new ClassB();
        try {
            aClass.identifyClass();
        }
        catch(Exception e){
            System.out.println("ClassA Method: Exception: "+e.getMessage());
        }
    }
    public class ClassB {
    public void identifyClass()throws Exception{
        System.out.println("ClassB identifyClass method: ");
        throw new Exception("  This looks into exception.");
    }
}
	
	
	
	
