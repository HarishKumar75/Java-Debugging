# Java-Debugging
1.)ArrayManipulation
public class ArrayManipulation {
	 public static void main(String[] args) {
	        int[] numbers = {1, 2, 3, 4, 5};
	        
	        for (int i = 0; i < numbers.length; i++) {
	            System.out.println(numbers[i]);
	        }
	    }
}

2.)Object-Oriented Programming
class Car {
    private String make;
    private String model;

    public Car(String make, String model) {
        this.make = make;
        this.model = model;
    }

    public void start() {
        System.out.println("Starting the car.");
    }
     
    public void stop() {
    	System.out.println("Stopping the car.");
    }
}

public class Main1 {
    public static void main(String[] args) {
        Car car = new Car("Toyota", "Camry");
        car.start();
        car.stop();
    }
}

3.) Exception Handling

public class ExceptionHandling {
	public static void main(String[] args) {
        int[] numbers = {1, 2, 3, 4, 5};
        
        try {
            System.out.println(numbers[10]);
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Array index out of bounds.");
        }
        
        int a=10;
        int b=0;
        
        try {
        	int result=divide(a,b);
        	System.out.println("Results:"+result);
        	
        } catch(ArithmeticException e) {
        	System.out.println("Divison by zero is not allowed.");
        }
	
    }

    public static int divide(int a, int b) {
    	if(b==0) {
    		throw new ArithmeticException("Divison by zero is not allowed.");
    	}
