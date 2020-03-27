## Stacks & Queues

**Stacks**  
Stacks are data structures of Nodes. Nodes reference the next node but do not reference the previous node. Stacks follow FILO and LIFO.
Terminology for Stack:
1. *Push* O(1)  
    - Nodes/items that are put into the stack are pushed. 
    - will always be O(1) because no matter how many nodes you have in the stack, it takes the same amout of time.
    - When you push a node, it is assigning it as a new top with next equalling to the original top.
    - first have a node to add to the stack, then assign the next property of your node to reference the same node top is referencing to. Lastly, reassign the reference top to the new node.
    - Syntax:
    ```
    Node.next <-- Top  
    top <--- Node
    ```
2. *Pop* O(1)  
    - Nodes/Items that are removed from the stack, if you try to pop and empty stack, there will be an exception
    - When using the pop, the top node is returned to the user
    - Before popping, you should check if the stack `isEmpty`
    - First create a reference named `temp` that points to  the same node `top` does, then reassign top to point to the value `next` is point to.  Then clear out the next property in your current temp reference. Lastly return the temp node.
    ```
    Node temp <-- top  
    top <-- top.next  
    temp.next <-- null  
    return temp  
    ```
3. *Top* - Top of the stack
4. *Peek* O(1)  
    - Allows you to view the top Node in the stack, if it's an empty stack, there will be an exception.
    - First check `isEmpty` before peeking. For peek, we don't reassign the next property
    - `return top.value`
5. *isEmpty* O(1)  
    - returns true when the stack is empty
    - `return top != null`
 

**Queue**  
Queues follow FIFO and LILO.
1. *Enqueue* 
    - Node/Items that are added 
    - First change next property of the rear node to point to the node we are going to add. Then assign the rear nodes `next` to the one you are adding. Then reassign rear to the newly added node
    ```
    rear.next <-- Node
    rear <-- Node
    ```
2. *Dequeue*
    - nodes/items that are removed, which is always the front node
    - First checked isEmpty then create a temp reference and point to the same node that front is. Then reassign front to the next value that front is referencing. Lastly reassign the next property on temp null to null
    ```
    Node temp <-- front
    front <-- front.next
    temp.next <--null
    return temp
    ```
3. *Front* 
    - first node of the queue
4. *Rear*
    - last node of the queue
5. *Peek*
    - you view the front node
    - first check isEmpty
    - `return front.value`
6. *IsEmpty*
    - returns true when empty
    - `return front != null`

