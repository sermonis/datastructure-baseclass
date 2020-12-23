# dataStructure-baseClass
Basic classes commonly used in data structures

## Array
### Output array as string
* join connects all array elements into a string
* toString returns the array as a string
* valueOf is similar to toString, returning the array as a string

### @@iterator
* @@iterator returns an iterator object containing array key-value pairs, which can be called by synchronously to get the key-value pairs of array elements
* entries return @@iterator containing all key-value pairs of the array
* keys return @@iterator containing all indexes of the array
* values returns @@iterator containing all the values in the array

### Fill the array
* copyWithin copies a series of elements in the array to the specified starting position of the same array
* fill fills the array with static values
* from creates a new array based on the existing array
* of creates a new array based on the parameters passed in
* slice passes in the index value, and returns the elements in the corresponding index range in the array as a new array

### Array merge
* concat connects 2 or more arrays and returns the result

### Iterator function
* some runs the given function on each item in the array, if any item returns true, it returns true
* every runs the given function for each item in the array, if the function returns true for each item, it returns true
* map runs a given function on each item in the array and returns an array composed of the results of each function call
* filter runs a given function on each item in the array, and returns an array of items that the function returns true
* forEach runs the given function on each item in the array. This method has no return value
* The reduce method receives a function as a parameter. This function has four parameters: previousValue, currentValue, index and array. This function will return a value that will be added to the accumulator, which will be returned after the reduce method stops executing. This is useful if you want to sum all the elements in an array

### Search for
* indexOf returns the index of the first array element equal to the given parameter, or -1 if not found
* lastIndexOf returns the largest value in the index of the element equal to the given parameter searched in the array
* includes returns true if there is an element in the array, otherwise it returns false. ES7 new
* find finds an element from the array according to the conditions given by the callback function, and returns the element if found
* findIndex finds an element from the array according to the conditions given by the callback function, and returns the index of the element in the array if found

### Sort
* sort sorts the array in alphabetical order, supports passing in the function of the specified sorting method as a parameter
* reverse reverses the order of the elements in the array, the original first element now becomes the last, and the original last element becomes the current first

## Stack
> The actual application of the stack is very extensive. In the backtracking problem, it can store tasks or paths that have been visited, and undo operations
* A stack is an ordered collection that complies with the LIFO principle.
* Newly added or to-be-deleted elements are stored on the same end of the stack, called the top of the stack, and the other end is called the bottom of the stack. In the stack, new elements are close to the top of the stack, and old elements are close to the bottom of the stack.

## Queue
> Queue is a group of ordered items following the FIFO (First In First Out, also known as first come first serve) principle. The queue adds new elements at the end and removes elements from the top. The newly added element must be at the end of the queue.
* When you open a new tab in the browser, a task queue will be created. This is because each tag handles all tasks in a single thread, and it is called an event loop. The browser is responsible for multiple tasks, such as rendering HTML, executing JavaScript code, handling user interaction (user input, mouse clicks, etc.), and executing and processing asynchronous requests.
* The realization of two very famous special queues: priority queue and circular queue.

## LinkedList
> The size of the array is fixed, and the cost of inserting or removing items from the beginning or middle of the array is high because of the need to move elements.
>The linked list stores an ordered collection of elements, but unlike an array, the elements in the linked list are not placed consecutively in memory. Each element consists of a node that stores the element itself and a reference (also called a pointer or link) to the next element.
* Compared to traditional arrays, one advantage of linked lists is that there is no need to move other elements when `add` or `remove` elements. However, the linked list requires the use of pointers, so additional attention is required when implementing the linked list.
* Another detail of the array is that you can `directly access any element in any position`, and to access an element in the middle of the linked list, you need to iterate the list from the `start point (head of the list) until you find the desired element`
* Singly linked list and doubly linked list

## Set
> Do not allow duplicate objects

**The following operations can be performed on the collection. **
+ Union: For the given two sets, return a new set containing all the elements in the two sets.
+ Intersection: For the given two sets, return a new set containing the elements in common in the two sets.
+ Difference set: For the given two sets, return a new set containing all the elements that exist in the first set but not in the second set.
+ Subset: verify whether a given set is a subset of another set.

## Dictionary
> A set represents a group of different elements (not repeating elements). In the dictionary, [key, value] pairs are stored, where the key name is used to query specific elements. Dictionaries are very similar to sets. Sets store elements in the form of [value, value], and dictionaries store elements in the form of [key, value]. Dictionaries are also called mappings.
### HashMap
It is a hash table implementation of the Dictionary class. The purpose of the hash algorithm is to find a value in the data structure as quickly as possible.
Generally, if you want to get a value in a data structure (using the get method), you need to traverse the entire data structure to find it. If you use a hash function, you know the specific location of the value, so you can quickly retrieve the value.
The function of the hash function is to give a key value and then return the address of the value in the table.

## binary-tree
> A non-sequential data structure-tree, which is very useful for storing data that needs to be quickly found
* Preorder traversal: can be used to display the directory structure
* Post-order traversal: It can be used as an expression tree, and users can implement basic addition, subtraction, multiplication and division when implemented at the bottom of the compiler, such as a*b+c
* Post-order traversal: calculate the size of the space occupied by all files in a directory and its subdirectories
