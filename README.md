# Java-Memory_Manipulation_Protection
The perfect little Java libary to protect your java number values.

This is the perfect little libary for java developers to protect your java values.
If you are using this libary you can prevent that cheaters can manipulate the memory adress values
of you java application.



Example Main class:



public class Main {

	public static ValueAntiCheat valueAntiCheat;  //create object valueAntiCheat
	public static Value value_1; //create Values how much you want have protected
	public static Value value_2; //in this case 3
	public static Value value_3;
	
	public static void main(String[] args) {

		valueAntiCheat = new ValueAntiCheat(2000);
    //initialize valueAntiCheat and establish the delay through attempts of checking the values
		
		value_1 = new Value("value1", 5); //initialize all your Values
		value_2 = new Value("value2", 25);
		value_3 = new Value("value3", 50);
		
		valueAntiCheat.addValue(value_1); //add all Values to the valueAntiCheat
		valueAntiCheat.addValue(value_2);
		valueAntiCheat.addValue(value_3);
		
		valueAntiCheat.readyToCheck(); //if you have done that all do this

	}

}
