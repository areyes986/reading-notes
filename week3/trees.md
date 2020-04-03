## Trees
Terminology:  
1. Node - individual item/data, makes up the data structure
2. Root - first//top Node in tree
3. Left Child - node that is to the left of a root or node
4. Right Child - node that is to the right of a root or node
5. Edge -  link between child and parent node
6. Leaf - node that doesnt have children
7. Height - height is the # of edges from root to bottommost node

We use recursion to traverse through trees and it relies on the call stack to go back up the tree when you're at the end of a subpath.
Two categories of traversal:  
1. Depth First 
    - prioritizes going through the DEPTH(height) of the tree. 
    - *pre-order:* `root>>left>>right`
        - the ROOT IS LOOKED AT FIRST. 
        - when called for the first time, the root is added to the call stack
        - then it checks if the root has a left node and if it does, that will be added to the call stack
        - after that, the left child will be popped off and go back up to the parent
        - then it will check for right and after finding the right child, it will pop and go back up to the same parent
        - if there are no more children left, that parent will pop off the stack to and go back up to the root.
        - the root will then look for a right child and when everything is popped, it will eventually go back up to the root  
        ```
        Output <-- node.value
        if (root.left != null)
        preOrder(root.left)
        if (root.right != null)
        preOrder(root.right)
        ```
    - *in-order:* `left>>root>>right`
        ```
        if (node.left != null)
        inOrder(node.left)
        output <-- node.value
        if (node.right != null)
        inOrder(node.right)
        ```
    - post-order: `left>>right>>root`
        ```
        if (node.left != null)
        inOrder(node.left)
        if (node.right != null)
        inOrder(node.right)
        output <-- node.value
        ```
2. Breadth First
    - Traversal iterates through the tree by going through each lvl of the tree node-by-node. Breadth First uses a queue to traverse the width of the tree.
        - you first but the root into the queue
        - then you dequeue that node and we can use it in the code
        - after you dequeue, you enqueue the next lvl from left child to right child
        - left child will be the new front and we repeat that same process as before with that root
        - then keep going until there are no children and we can just dequeue without enqueuing more
        ```
        Queue breadth <-- new Queue()
        breadth.enqueue(root)
        while breadth.peek()
        node front = breadth.dequeue()
        Output <-- front.value
        if (front.left != null)
        breadth.enqueue(front.left)
        if(front.right != null)
        breadth.enqueue(front.right)
        ```

         

        
