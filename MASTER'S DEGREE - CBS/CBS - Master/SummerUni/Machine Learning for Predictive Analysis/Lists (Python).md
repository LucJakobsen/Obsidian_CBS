Lists are the most commonly used [[Data Structures (Python)|Data Structure]]. Think of it as a sequence of data that is enclosed in square brackets and data are separated by a comma.

Each value can be accessed by calling its index value, which is done through [[Indexing (Python)]].
If you want to access a sequence of data you can perform [[Slicing (Python)]]. 

Lists are declared by equating a variable to ``[]``

Lists can contain many items


### Built-in List Functions
- ``len()`` will return the length/number of items of the list
- ``min()`` will return the minimum value in the list
- ``max()`` will return the maximum value in the list
- ``append()`` can be used to add an entire list at the end
	- But if nested list is not wanted you can instead use ``extend()``
- ``count()`` is used to count the number of a particular element is present in the list
- ``index()`` is used to find the index value of a particular element
- ``insert(x,y)`` is inserts a value but does replace the element
	- if you want to replace an element simply assign it a new value instead
- ``pop()`` used to remove elements based on its index value, which can be assigned to a variable
	- If you just use pop without specifying it will remove the last item in the list
	- You can also remove an element by specifying the element itself using ``remove()``
- ``reverse()`` used to reverse the elements in the list
- ``sort()`` used to sort the elements in a list in as specific order


- Lists can also be concatenated using ``+``

- To check if something is present in the list you can use ``in`` 
	- E.g. ``"Fire" in names`` will check if the string "Fire" is present in the list "names"


