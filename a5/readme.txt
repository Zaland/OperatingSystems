test1.c
----------------------------------------------------------------------------------------------
The first test case tests the working functions and the parts where it returns error messages.

Firstly it starts the memory with a certain amount of size that could fit all the grow_memory
functions to follow. One of the grow_memory functions is larger than it should be to return 
an error message to make sure that it doesn't work. There are 4 nodes and 3 are filled in
with the first node being the head, and the other two nodes are randomly chosen. The fourth
node is empty to confirm its function when used.

Second, the test file will grow and pregrow memory with the already defined nodes. It will 
try to grow and pregrow memory by a larger number and try to grow. Also try to grow an empty
node that will end up returning an error. After growing each node, then print the list to
see the change.

Third, try to release memory for the nodes that are already stored. The first three nodes will
end up releasing memory, and right after it releases a memory, it will print the list using its
memory size. It will also try to release memory to the empty node which will end up returning
an error. 

Finally, it will end the memory, releasing all memory leaks and then freeing the memory that 
was malloc'ed in the beginning.



test2.c
----------------------------------------------------------------------------------------------
The second test adds more get memory functions and doesn't test error messages.

Firstly it starts the memory with a certain size that can fit all the get memory functions.
It will not try to return any error messages. It will store a couple of the nodes including
the head and the tail in void variables. Then it will print the current list using the
memory size as the value to be printed.

Second, the test file will grow and pregrow memory with the already defined nodes. It will 
try to grow and pregrow memory by a larger number and try to grow. Also try to grow an empty
node that will end up returning an error. After growing each node, then print the list to
see the change. It will try to pregrow the final node to a smaller number to see the change.

Third, try to release memory for the nodes that are already stored. Release all nodes in 
order and then print the list every time memory is released.

Finally, it will end the memory, releasing all memory leaks and then freeing the memory that 
was malloc'ed in the beginning. 