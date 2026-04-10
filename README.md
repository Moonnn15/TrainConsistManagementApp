


Project Procedure – UC4: Maintain Ordered Bogie Consist
1. Continue the Project
Using the existing Java project and class TrainConsistManagementApp.java, extend the system to maintain the physical order of bogies in a train.

2. Display UC4 Title
Inside the main method, print:

==================================
UC4 - Maintain Ordered Bogie Consist
==================================
This indicates operations related to maintaining train sequence.

3. Introduce LinkedList
To manage ordered bogies efficiently:

Use the List interface

Use LinkedList implementation

List<String> trainConsist = new LinkedList<>();
Unlike ArrayList, LinkedList uses node connections, making insertions and deletions efficient.

4. Add Initial Bogies
Add bogies in sequence using .add():

trainConsist.add("Engine");
trainConsist.add("Sleeper");
trainConsist.add("AC");
trainConsist.add("Cargo");
trainConsist.add("Guard");
5. Display Initial Train Consist
Initial Train Consist:
[Engine, Sleeper, AC, Cargo, Guard]
This represents the initial arrangement of the train.

6. Insert a Bogie in the Middle
Insert Pantry Car at position 2 using:

trainConsist.add(2, "Pantry Car");
7. Display Updated Consist
After Inserting 'Pantry Car' at position 2:
[Engine, Sleeper, Pantry Car, AC, Cargo, Guard]
This demonstrates mid-list insertion efficiency.

8. Remove First and Last Bogies
Remove bogies from both ends:

trainConsist.remove(0); // Remove Engine
trainConsist.remove(trainConsist.size() - 1); // Remove Guard
9. Display Final Consist
After Removing First and Last Bogie:
[Sleeper, Pantry Car, AC, Cargo]
10. Completion Message
UC4 ordered consist operations completed...
Actor & Flow
Actor: User

Flow:

User defines bogie sequence

System stores bogies in LinkedList

Bogies are inserted at specific positions

First and last bogies are removed

Final ordered consist is displayed

Key Concepts Used in UC4
LinkedList – Doubly linked list implementation

Node Structure Concept – Each element links to previous and next nodes

add(index, element) – Insert at a specific position

remove() – Delete elements from list

Order Preservation – Maintains real-world train sequence

Key Requirements
Create a LinkedList<String> for train consist

Add bogies: Engine, Sleeper, AC, Cargo, Guard

Insert Pantry Car at position 2

Remove first and last bogies

Display the final ordered train consist

Key Benefits
Models real-world train arrangement

Efficient insertion and deletion compared to ArrayList

Helps understand node-based data structures

Demonstrates importance of order maintenance

Outcome of UC4
After completing this procedure:

Train bogies are maintained in a strict order

Insertions and deletions are handled efficiently

The system reflects real-world train composition behavior

The application demonstrates effective use of LinkedList for ordered data management
