# CalorieTracker
The project titled “Calorie Tracker” uses the Java Programming language and it utilizes the concepts of Association, Inheritance and Swing (for accessing the GUI tools).

The Calorie tracker is a window (created using the Swing package), which takes the input of age and Gender from the user. This window also consists of 4 categories (separated as columns) titled Breakfast, Lunch, Drinks and Dinner,
containing three food items pertaining to each field to represent all the meals/ foods consumed in a day. The user can enter the number of food items he/she has consumed next to the item’s name in each of these categories and on
clicking a button named “Submit”, the total number of calories in each of the fields along with the total number of calories consumed by the user throughout the day will be displayed. The user will also be able to view a message stating whether he/she is fit and active or not depending on the total number of calories.


<img width="267" alt="image" src="https://github.com/user-attachments/assets/62d6eba3-90fb-4003-af48-c81798ca96d9" />

Implementation: An abstract class “Food.java” consists of an abstract method titled food details which takes an integer array as the argument. Next, a class “FItems.java” has a String array “items” for the storing the ingredients of all the food items and a Double array “val” to store the values of calories for each of these ingredients per 100 ml / 100 gm (The element at index value ‘i’ in the String array has the calories stored at index value ‘i’ in the Double array). In the classes “Breakfast.java”, “LunchDinner.java” and “Drinks.java”, an Object of the FItems class is taken as an instance variable along with a String array “foods” and a Double array “fvalues”, respectively. In the constructors for each of these classes, the “foods” array is initialized with the names of the food items in that category. “fvalues” is a Double array of 3 elements (corresponding to the three food items) which contains the calories of each of the food items as a sum of the values of each of the ingredients with the quantity of the ingredient present in the food. Fvalues[i] = Ʃ (quantity of each ingredient) *(no. of calories for the ingredient) In the method “food details”, an integer array is passed as an argument with provides the quantity of each of the food items and this method returns a Double value containing the sum of the calories from all the food items.

In the class “AgeGen.java”, an integer “age” and a String “Gender” are taken as the Instance Variables. This class has a method getDetails(), with a Double value “cals” as an argument, which considers the gender and then uses if-else conditions to check the age and the minimum and maximum calories required for each of the age groups. If the calories value passed as the argument corresponding to the age conditions is satisfied, a string is returned with the message of the person (a baby, a child, a teen or an adult) being fit and active. Else, the string consists of a message indicating the use is not active.

Finally, in the most important class “CalorieCal.java”, the class inherits from Canvas and implements the ActionListener. The constructor of this class consists of a JFrame along with several JLabels, JTextFields and a JButton.


Developed by M. Bhagya Sree and S. Anusri
