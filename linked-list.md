## Linked Lists
It is a sequence of *Nodes*(elements of the list) that are connected to each other. Each node references the next node. Link Lists are linear/dynamic data structures. Useful when you do not know the sizing of the list and to just add/remove quickly.
Two Types of Linked List:  
1. **Singly**
    - number of references the node has
    - There is only ONE reference which points to the *next* node. 
    - Goes in one direction
    - Starts at the head then tranverses to the last node then ends at a null value.
2. **Doubly** 
    - Two/Double references within the node. 
    - References to the *next* and *previous* node.

Other terminology: 
**Next:** This is a property each node has and has the reference to the next node.  It leads us to the next node and lets us extract data. Guides us to where the next reference is pointing.  
**Head:** Reference type of type node to the first node in the list.  
**Current:** Reference type of type node. Is currently looked at. Typically reset current to the head to know you are starting from the beginning of list.  Tells us where we are in the list and lets us move forward until the end. We know we are all the end when the current is null.  
**Transversal:** You can't use a foreach or for loop when transversing. Best to do a while loop to always be checking that next node isn't null. If it does, the program crashes or ends.  
**Node:**  Elements of the list. They have data it holds and references to the next node.

**How to add a node**
Find the head node of the lists -> make new node and set pointer to current first node -> rearrange head node's pointer to the new node.
1. Set current equal to head.
2. Instantiate the new node that's being added using the `Add()` method with values in the parenths and define the next value of node.
3. `newNode.Next` is set to null and we set this property to the location the head is pointing to. 
4. Reassign where head is pointing to which is at newNode.

**How to add last node**
You add it after the last node. Find the last node and change the pointer -> create new node and set pointer to null -> direct preceding nodes pointer to new.

**Memory**  
Memory does not have live together, it can be scattered and does not need a set amount of memory. Size, shape, and amount and change.  
The nodes have the "address"/reference to the next node and do not have to be next to each other. 

**Drawbacks**
- Sometimes can be less efficients trying to search for a single element


