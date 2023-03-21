# Python Data Structure

## Lists and Tuples

Compound data types
#### Tuple
All kinds of data can be stored in one tuple.

- Slicing
- Immutable: if wanna change the tuple, need give variable a new tuple
- Nesting

#### List

- concatenate or combine lists by adding ("+"). 
- mutable : **Extend**( can extend a list [] at one go)
- Append: **append a list** instead a list of elements

![image-20230321175342240](./photo/image-20230321175342240.png)

- Del(A[4]) delete fourth element
- list.split(",")
- Clone: if i use b = a, then change b ,a will be changed as well

![image-20230321180038523](./photo/image-20230321180038523.png) 

![image-20230321180152322](./photo/image-20230321180152322.png)

## Dictionary

key can be any imuatble values even tuple: Dict[(0, 1)]

element = List[index]

Value = dictionary[key]  : key is analogous to the index

curly brackets {}

Add: DICT['Newkey'] = "value"

delete:  del(DICT['key'])



## Sets(no duplicate)

Collection: input different types

Unordered: do not record element position

Set.add("new element")

"element" in set

set1.union(set2)

Set1.issubset(set2)

album_set1 & album_set2

album_set1.difference(album_set2) 

album_set1.intersection(album_set2)  
