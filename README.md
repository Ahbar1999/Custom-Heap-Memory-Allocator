# Custom Heap memory allocator in C++


- overriding 'new' and 'delete' operators from the '<new>' header to take memory allocation into our own hands from the OS 

-The program starts with reserving 10 buckets of 1MB(page size) of memory
So basically our program has now total of 10MB of heap memory available but everytime you allocate a new object on heap you use up all of 1 bucket of memory which is 1 MB 

-So you can have at most 10 objects at any time in the program
After that you try if to allocate more memory it will throw a 'bad-alloc' exception 
