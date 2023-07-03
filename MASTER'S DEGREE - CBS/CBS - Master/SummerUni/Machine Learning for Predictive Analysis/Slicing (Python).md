Slicing is used to access a sequence of data in a [[Lists (Python)|list]].

It is done by specifying the start position `start` and end position `stop` of the selection. Written as `[start:stop]`

**Example:**
Input: 
``num = [2, 4, 1, 6, 5, 6, 0, 9, 8]``
``num``
Output:
``[2, 4, 1, 6, 5, 6, 0, 9, 8]``

Input:
``num[0:4]``
Output:
``[2, 4, 1, 6]``

Input:
``num[4]
Output:
``5

If ``start`` is omitted the selection is made from the beginning, and if ``stop`` is omitted the selection is made up to the end. If both are omitted all items are selected.