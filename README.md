
Project Procedure – UC2: Add Passenger Bogies to Train
1. Continue the Project
Using the existing Java project created in IntelliJ IDE and the class TrainConsistManagementApp.java, we extend the functionality to manage passenger bogies.

2. Display UC2 Title
Inside the main method, display the module heading using console output:

==================================
UC2 - Add Passenger Bogies to Train
==================================
This informs the user that the application is now performing operations related to passenger bogies.

3. Initialize Passenger Bogie List
Create a dynamic list to store passenger bogies:

Use the List interface for abstraction.

Use the ArrayList class for dynamic resizing.

List<String> passengerBogies = new ArrayList<>();
This list will hold different types of passenger bogies.

4. Add Passenger Bogies
Add different types of bogies using the .add() method:

Sleeper

AC Chair

First Class

passengerBogies.add("Sleeper");
passengerBogies.add("AC Chair");
passengerBogies.add("First Class");
5. Display Added Bogies
Print the list after adding bogies:

After Adding Bogies:
Passenger Bogies : [Sleeper, AC Chair, First Class]
This confirms successful insertion into the dynamic list.

6. Remove a Bogie
Remove a specific bogie using the .remove() method:

passengerBogies.remove("AC Chair");
7. Display Updated List
Print the list after removal:

After Removing 'AC Chair':
Passenger Bogies : [Sleeper, First Class]
This demonstrates dynamic deletion capability.

8. Check Bogie Availability
Use the .contains() method to verify if a bogie exists:

passengerBogies.contains("Sleeper");
Output:

Contains Sleeper? : true
9. Display Final Passenger Consist
Print the final state of the passenger bogie list:

Final Train Passenger Consist:
[Sleeper, First Class]
10. Completion Message
Display a confirmation message:

UC2 operations completed successfully...
Outcome of UC2
After completing this procedure:

Passenger bogies are successfully added to the train consist.

A specific bogie is removed dynamically.

The system verifies the presence of a bogie using search functionality.

Final passenger consist is displayed accurately.

The application demonstrates effective use of ArrayList operations such as add, remove, and contains.


