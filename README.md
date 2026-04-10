


Project Procedure – UC5: Preserve Insertion Order of Bogies
1. Continue the Project
Using the existing Java project and class TrainConsistManagementApp.java, extend the system to maintain both uniqueness and insertion order of bogies.

2. Display UC5 Title
Inside the main method, print:

==================================
UC5 - Preserve Insertion Order of Bogies
==================================
This indicates that the system now focuses on ordered and unique train formation.

3. Identify the Need
From previous use cases:

HashSet (UC3) ensures uniqueness but does not maintain order

LinkedList (UC4) maintains order but allows duplicates

👉 We need a structure that:

Prevents duplicates

Preserves insertion order

4. Introduce LinkedHashSet
To achieve both goals:

Use the Set interface

Use LinkedHashSet implementation

Set<String> formation = new LinkedHashSet<>();
LinkedHashSet combines:

Hashing (for uniqueness)

Linked list (for order preservation)

5. Add Bogies
Insert bogies using .add():

formation.add("Engine");
formation.add("Sleeper");
formation.add("Cargo");
formation.add("Guard");
6. Add Duplicate Entry
Intentionally add a duplicate:

formation.add("Sleeper"); // Duplicate
7. Observe Behavior
Duplicate entry is ignored automatically

Original insertion order is preserved

8. Display Final Train Formation
Final Train Formation:
[Engine, Sleeper, Cargo, Guard]
9. Display Informational Note
LinkedHashSet preserves insertion order and removes duplicates automatically.
10. Completion Message
UC5 formation setup completed...
Actor & Flow
Actor: User

Flow:

User adds bogie names

System inserts them into LinkedHashSet

Duplicate entries are ignored

Insertion order is preserved

Final formation is displayed

Key Concepts Used in UC5
Set Interface – Ensures no duplicate elements

LinkedHashSet Class – Maintains insertion order

add() Method – Inserts elements

Automatic Deduplication – No manual validation required

Order Preservation – Maintains sequence of insertion

Key Requirements
Create a LinkedHashSet<String> for train formation

Add bogies: Engine, Sleeper, Cargo, Guard

Add duplicate value intentionally

Print final formation

Verify:

No duplicates

Order is preserved

Key Benefits
Combines uniqueness + order preservation

Prevents duplicate bogie entries

Maintains realistic train sequence

Demonstrates when to use LinkedHashSet over HashSet and List

Outcome of UC5
After completing this procedure:

Train formation maintains unique bogies only

Original insertion sequence is retained

Duplicate entries are automatically eliminated

The application demonstrates effective use of LinkedHashSet for ordered and unique data management
