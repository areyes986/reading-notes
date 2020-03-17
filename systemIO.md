## System.IO
**File and Stream I/O**  
This is the transfer of data to or from a storage medium. `System.IO` namespace  has types that enable reading/writing on data streams and files. We can use types in the System.IO namespace so we can interact with files/directories. 
Commonly Used file and directory classes:
- file - helps with creating, copying, deleting, moving, and opening files
- fileinfo - helps provide instance methods for same as above
- directory - static method for creating, moving, and enumerating thorugh sub/directories
- directoryinfo - instance method for same as above
- path - methods/properties for processing directory string in a cross-platform manner.
**Streams**
A stream is a system of bytes that is used to read/write to a backing store such as disks or memory. There are many kinds of streams other than files like network, memory, and pipe streams. The Stream class provide a common view of data resoures/repos. The programmer is isolated from certain details of OS and underlying devices. Common stream classes can be found in the reading [link](https://docs.microsoft.com/en-us/dotnet/standard/io/)
Streams and 3 fundamental operations:  
1. Reading - transfers data from stream to data stucture like array of bytes
2. Writing - transfers data to a stream from data source
3. Seeking - querying/modifying current position within a stream.

Reader and Writer types handle conversation from encoded characters to and from bytes. They are associat4ed with stream that can be retrieved through class's BaseStream property.

**Write and Read to a file**
System.IO.BinaryWriter and System.IO.BinaryReader classes write and read data other than character strings
These classes and methods are usually used to write to a file:
- StreamWriter - has methods to write to a file sychronously or asynchronously
- File - helps static method to write to a file or append text to it. These method examples are WriteAllLines or AppendAllLines
- Path - this is for strings that have a file or directory path info. It has the Combine method, Join, and TryJoin.  
[Link to Writing](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-write-text-to-a-file)  
[Link to Reading](https://docs.microsoft.com/en-us/dotnet/standard/io/how-to-read-and-write-to-a-newly-created-data-file)


