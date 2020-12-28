# SortedList vs SortedDictionary

|  SortedList  | SortedDictionary  |
| ------------ | ------------ |
|  The SortedList is implemented by using two Arrays, one containing the keys and the other one containing the values. |  The SortedDictionary is implemented as a Binary Search Tree. |
| Once sorted, It is faster in the retrieval of data.  |  It is faster in insertion and removing key-value pairs. |
| Access elements using the index is possible.  | Access elements using the index or key is possible.  |
| The elements are stored in a continuous block in memory. |  The elements are stored in separate object that can spread all over the heap. |
| The memory fragmentation is high.  | The memory fragmentation is low.  |

**Common Characteristics with respect to key and value for both SortedList and SortedDictionary:**
* All keys should be unique and not null.
* A value can be null or duplicate.
* If keys are strings, they will be case sensitive.
* It doesn’t allow to add any other type than declared.
* Key/Values pairs are stored as a KeyValue Pair object.

**When should use one and not the other?** 

* If you need to access items using their index within the collection
* If you are populating the dictionary all at once from sorted data
* If you aren’t adding or removing keys once it’s populated
**_Then use a SortedList._**

* If you don’t know how many items are going to be in the dictionary?
* If you are populating the dictionary from random, unsorted data
* If you are adding & removing items randomly
**_Then use a SortedDictionary._**