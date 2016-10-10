# CSCI-232-Lab-2
CSCI Lab 2 repository

What we need to do:

1) Create a Hashtable that is an array of Trees:
2) create operation and main classes for methods and use.

Main method set up: (use something similar to the old main method?)
	“Enter size of hash table: ”
	“Enter initial number of items: ”
	“Enter first letter of show, insert, or find: ”
		“Enter key value to (insert/find)”
Hash function: H(x) = x%arraySize

arraySize must be an input parameter


Methods (descriptive, how-to):

Insert Method: Set method to create a tree when array index is null, and set root as your input data; when not null (there is already a tree) call an insert method for binary search tree. Set if statement “if input == node.getValue and delete flag not true, break out of method” (so we don’t add duplicates); else flip flag to false(to reinsert value if previously deleted).
	
	^^Prevent duplicates from being inserted. (see insert method)

Search Method: Apply hash function to value to be searched; go into array at index directed by hash function; go down tree same as if insert looking for where to put it; if searched item==current.getvalue and delete flag is false, return found; if current.getvalue == null or ==current.getvalue and delete flag is true, return not present.

Display Method: Use an inorder traversal of each tree, printing exactly as in first lab except that it should check if delete flag is true, in which case it should skip print statement for that node.

Delete method: Set additional boolean variable to each tree node, “deleted”, starts as false. When deleting, swap flag.
	
	^^Don’t need to do deletion (but 10 bonus points if we do)





