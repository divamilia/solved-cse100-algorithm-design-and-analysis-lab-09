Download Link: https://assignmentchef.com/product/solved-cse100-algorithm-design-and-analysis-lab-09
<br>
<strong>Hash Table with Chaining</strong>

In this assignment you are requested to implement a hash table that handles collisions with chaining. You have to use linked lists, either from the Standard Template Library (STL) (recommended) or by implementing your own. For usage of STL, refer for instance to <a href="http://www.cppreference.com/wiki">here.</a>

You have to implement the insert, search and delete operations. The keys are integers (C++ int type) and you can assume that all keys <em>k </em>are non-negative. The first number in the input will be the size <em>m </em>of the chained hash table. You will use the simple hash function <em>h</em>(<em>k</em>) = <em>k </em>mod <em>m</em>.

The input contains one of the following commands on a line:

<ul>

 <li>i key: Insert key into the hash table. For example, “i 2” means “Insert key 2 into the hash table”. For collisions, insert the colliding key at the beginning of the linked list. You just need to insert the key and do not have to output anything in this case.</li>

 <li>d key: Delete key from the hash table. For example, “d 2” means “Delete key 2 from the hash table”. Do nothing if the hash table does not contain the key. If there are multiple elements with the same key value, delete just one element. If the delete is successful, you have to output: key : DELETED</li>

</ul>

If not (since there was no element with the given key), output:

key : DELETE FAILED

<ul>

 <li>s key: Search key in the hash table. If there is an element with the key value, then you have to output:</li>

</ul>

key : FOUND AT i,j

where <em>i </em>is the hash table index and <em>j </em>is the linked list index. If there are multiple elements with the same key value, choose the first one appearing in the linked list. If you do not find the key, then output:

key : NOT FOUND

<ul>

 <li>o: Output the hash table. Output the entire hash table. Each line should begin with the slot/hash table index followed by key values in the linked list. For example, if <em>m </em>= 3 and we inserted 3, 6, and 1 into an empty table in this order, then you should output:</li>

</ul>

0 : 6-&gt;3 1 : 1 2 :

<ul>

 <li>e: Finish your program.</li>

</ul>