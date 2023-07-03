Dictionaries are a type of [[Data Structures (Python)|data structure]] which contain a list of definitions that correspond to unique terms.

Dictionaries are unordered.

Creating a dictionary is done using curly brackets ``{}``

Similarly to [[Lists (Python)]] you can use square brackets to access elements/values in a dictionary ``[]``



**Example:**
``city_population = {
    ``"Tokyo": 13350000,  # a key-value pair
    ``"Los Angeles": 18550000,
    ``"New York City": 8400000,
   `` "San Francisco": 1837442,
``}
``print(city_population)
``print(type(city_population))``

Say you want to know the population of New York. Similarly to a list, you can use brackets to access the value, but this time with the key (instead of the index):
- ``city_population["New York City"]`` will return ``8400000``

