

Project Procedure – UC3: Track Unique Bogie IDs
1. Continue the Project
Using the existing Java project and class TrainConsistManagementApp.java, extend the application to enforce uniqueness of bogie IDs.

2. Display UC3 Title
Inside the main method, print the heading:

==================================
UC3 - Track Unique Bogie IDs
==================================
This indicates that the system is now validating uniqueness of bogie identifiers.

3. Identify the Drawback of UC2
In UC2, a List was used to store bogies.

Lists allow duplicate values

Example issue:

BG101, BG101
This can lead to:

Invalid train composition

Data inconsistency

Safety risks

4. Introduce Set for Uniqueness
To solve this problem:

Use the Set interface

Use HashSet implementation

Set<String> bogies = new HashSet<>();
A HashSet automatically ensures that all elements are unique.

5. Add Bogie IDs (Including Duplicates)
Insert bogie IDs using the .add() method:

bogies.add("BG101");
bogies.add("BG102");
bogies.add("BG103");
bogies.add("BG104");
bogies.add("BG101"); // Duplicate
bogies.add("BG102"); // Duplicate
6. Observe Automatic Deduplication
When duplicates are added:

HashSet ignores duplicate entries automatically

No error is thrown

Only unique values are stored internally

7. Display Bogie IDs
Print the set:

Bogie IDs After Insertion:
[BG101, BG102, BG103, BG104]
(Note: Order may vary because HashSet is unordered.)

8. Display Informational Note
Duplicates are automatically ignored by HashSet.
9. Completion Message
UC3 uniqueness validation completed...
Actor & Flow
Actor: User

Flow:

User adds bogie IDs

System inserts them into HashSet

Duplicate values are ignored automatically

Unique bogie IDs are displayed

Key Concepts Used in UC3
Set Interface – Collection that does not allow duplicates

HashSet Class – Implements Set using hashing

add() Method – Adds elements to the set

Automatic Deduplication – No manual checking required

Unordered Storage – Elements are not stored by index

Key Requirements
Create a HashSet<String> for bogie IDs

Add duplicate values intentionally

Print the final set

Verify that duplicates are removed automatically

Key Benefits
Enforces business constraints (unique bogie IDs)

Prevents data corruption and duplication errors

Demonstrates when to use Set instead of List

Introduces real-world validation logic in railway systems

Outcome of UC3
After completing this procedure:

Only unique bogie IDs are stored in the system

Duplicate entries are automatically eliminated

The train consist becomes more reliable and error-free

The application demonstrates effective use of HashSet for uniqueness enforcement


