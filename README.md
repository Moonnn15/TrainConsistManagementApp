Project Procedure – UC1: Initialize Train and Display Consist
1. Start the Project
Create a new Java project Intellij.
Add a new Java class named TrainConsistManagementApp.
2. Define the Class Structure
Inside the class, define the main method:
This is the starting point of the program.
The JVM begins execution from here.
3. Display Welcome Message
Use console output (System.out.println) to show:

=== Train Consist Management App ===
This informs the user that the application has started.
4. Initialize Train Consist
Create a dynamic list to store bogies.
Use:
List interface for flexibility.
ArrayList class for dynamic resizing.
Initially, the list should be empty (no bogies attached yet).
5. Confirm Initialization
Print a message indicating:
Train consist has been successfully initialized.
6. Display Initial Bogie Count
Use the .size() method on the list.
Since no bogies are added yet, it should display:

Initial bogie count: 0
7. Ensure Program Continuity
Keep the program running structure ready for future features.
This prepares the app for:
Adding bogies
Managing passenger and goods data
Safety checks
 Outcome of UC1
After completing this procedure:

The application starts successfully.
Train consist is created as an empty dynamic collection.
Initial state (bogie count = 0) is displayed to the user.
