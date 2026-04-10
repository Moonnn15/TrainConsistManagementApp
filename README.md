


Project Procedure – UC6: Map Bogie to Capacity (HashMap)
1. Continue the Project
Using the existing Java project and class TrainConsistManagementApp.java, extend the system to associate each bogie with its seating or load capacity.

2. Display UC6 Title
Inside the main method, print:

==================================
UC6 - Map Bogie to Capacity (HashMap)
==================================
This indicates that the system is now handling bogie attributes using key–value mapping.

3. Introduce HashMap
To map bogies with their capacities:

Use the Map interface

Use HashMap implementation

Map<String, Integer> capacityMap = new HashMap<>();
This structure stores:

Key → Bogie Name

Value → Capacity

4. Add Bogie-Capacity Mapping
Insert values using the .put() method:

capacityMap.put("First Class", 24);
capacityMap.put("Cargo", 120);
capacityMap.put("Sleeper", 72);
capacityMap.put("AC Chair", 56);
5. Display Heading
Bogie Capacity Details:
6. Iterate Using entrySet()
Loop through the map to access both key and value:

for (Map.Entry<String, Integer> entry : capacityMap.entrySet()) {
    System.out.println(entry.getKey() + " -> " + entry.getValue());
}
7. Display Output
First Class -> 24
Cargo -> 120
Sleeper -> 72
AC Chair -> 56
(Note: Order may vary since HashMap is unordered.)

8. Completion Message
UC6 bogie-capacity mapping completed...
Actor & Flow
Actor: User

Flow:

User creates bogie-capacity mapping

System stores data in HashMap

Key–value pairs are inserted using put()

System iterates using entrySet()

Bogie capacities are displayed

Program continues

Key Concepts Used in UC6
Map Interface – Stores key–value relationships

HashMap Class – Efficient key-based storage using hashing

put() Method – Inserts mappings

Key–Value Association – Links bogie to its capacity

entrySet() Iteration – Access both key and value together

Fast Lookup – Retrieve capacity using bogie name

Key Requirements
Create a HashMap<String, Integer>

Insert bogie capacities (Sleeper, AC Chair, First Class, Cargo)

Use put() for mapping

Iterate using entrySet()

Display bogie and capacity

Key Benefits
Models real-world attribute mapping

Introduces key–value data structures

Enables fast lookup and validation

Builds foundation for data-driven applications

Prepares for advanced analytics and planning systems

Outcome of UC6
After completing this procedure:

Each bogie is successfully mapped to its capacity

Data is stored in an efficient key–value structure

The system supports quick retrieval of bogie details

The application demonstrates effective use of HashMap for real-world data modeling
