# Built-in-List-Functions-in-python

DAte 14/06/2021:

1..)
append(x)
Add a single item to the end of the list
Equivalent to a[len(a):] = [x]
x = ['a', 'b', 'c', 'd']
x.append('e')
print(x)
['a', 'b', 'c', 'd', 'e']
x = ['a', 'b', 'c', 'd']
x.append([1, 2, 3])
print(x)
['a', 'b', 'c', 'd', [1, 2, 3]]
Click on  button to know how to append elements to List in Python.

extend(iterable)
Extend the list with the items of another list or iterable
Equivalent to a[len(a):] = iterable
x = ['a', 'b', 'c', 'd']
y = [1, 2, 3, 4]
x.extend(y)
print(x)
['a', 'b', 'c', 'd', 1, 2, 3, 4]
insert(index, item)
Insert an item at a position before the element given by index.
a.insert(0, x) inserts at the front of the list.
a.insert(len(a), x) is equivalent to a.append(x) which inserts an element at the end of list.
x = ['a', 'b', 'c', 'd']
x.insert(0, 1)
print(x)
[1, 'a', 'b', 'c', 'd']
x.insert(len(x), 'e')
print(x)
[1, 'a', 'b', 'c', 'd', 'e']remove(element)
Remove the first item in the list whose value is element
Error if the item doesn't exist with the value element in list
L1 = [1, 'a', 'b', 'c', 'd', 'e']
L1.remove(1)
print(L1)
['a', 'b', 'c', 'd', 'e']
L1.remove('f')
Traceback (most recent call last):
  File "", line 1, in 
ValueError: list.remove(x): x not in listpop(), pop(index)
Removes an item at the given position specified by index
Removes and returns the last element if index is not specified
If an invalid index is specified, then an IndexError is thrown
x = ['a', 'b', 'c', 'd', 'e']
x.pop(2)
'c'
print(x)
['a', 'b', 'd', 'e']
x.pop()
'e'
print(x)
['a', 'b', 'd']
x.pop(-1)
'd'
print(x)
['a', 'b']
x.pop(3)
Traceback (most recent call last):
  File "", line 1, in 
IndexError: pop index out of rangecount(x)
Return the number of times the item x appears in the list
x = ['a', 'b', 'a', 'c', 'd', 'e', 'a']
x.count('a')
3sort(key = None, reverse = False)
Sort the items of the list in place in ascending order
If the parameter reverse = True, then the list is sorted in place in descending order.
x = ['z', 'f', 'e', 'a','b', 'g', 't']
x.sort()
print(x)
['a', 'b', 'e', 'f', 'g', 't', 'z']
x.sort(key = None, reverse = True)
print(x)
['z', 't', 'g', 'f', 'e', 'b', 'a']reverse()
Reverse the order of elements of the list in place
x = ['z', 'f', 'e', 'a','b', 'g', 't']
x.reverse()
print(x)
['t', 'g', 'b', 'a', 'e', 'f', 'z']
copy()
Return the shallow copy of the list
Equivalent to a[:]
x = ['z', 'f', 'e', 'a','b', 'g', 't']
y = x.copy()
print(y)
['z', 'f', 'e', 'a', 'b', 'g', 't']
print(x is y)
False

 
 
 
 
 
