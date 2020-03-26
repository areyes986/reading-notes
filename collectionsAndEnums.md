## Collections and Enums
**Collections**  
Collections is a class and to use it, you must declare instances of the class before you can add on to it. Collections give flexibilty to working with a group of objects. The group of objects are able to grow/shrink dynamically. We can use keys that are put into the collection to an object so that we can retrieve the object using a key. Here are some common used classes of `System.Collections.Generic` namespace:
1. `Dictionary<TKey,TValue>` - represents key/value pairs
2. `List<T>` - Represents a list of objects that can be accessed by an index. Lets us search, sort, and modify lists.
3. `Queue<T>` - FIFO collection of objects
4. `SortedList<TKey,TValue>` - collection of key/value pairs. Sort by ket based on the `IComparer<T>` implementation.
5. `Stack<T>` - LIFO collection of objects.

**Enums**
This is a *value type* defined by set of underlying numerical types. The default values are integers and they start with zero and increase by one as the list goes on. But you can explicitly specify other integer types if you so choose. You cant define methods inside an enumeration type. 
