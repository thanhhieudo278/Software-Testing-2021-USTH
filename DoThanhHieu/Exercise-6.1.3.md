Exercise 6.1.3 Answer the following questions for the method search() below:

public static int search (List list, Object element)
// Effects: if list or element is null throw NullPointerException
// else if element is in the list, return an index
// of element in the list; else return -1
// for example, search ([3,3,1], 3) = either 0 or 1
// search ([1,7,5], 2) = -1
Base your answer on the following characteristic partitioning:

Characteristic: Location of element in list
Block 1: element is first entry in list
Block 2: element is last entry in list
Block 3: element is in some position other than first or last


a) “Location of element in list” fails the disjointness property. Give an example that illustrates this:

If the list has only one element, the element is both the first and the last entry. This violates the disjointness property.

b) “Location of element in list” fails the completeness property. Give an example that illustrates this:

It fails the completeness property because it lacks the case where the element is not in the list.

c) Supply one or more new partitions that capture the intent of “Location of element in list” but do not suffer from completeness or disjointness problems:

Block 1: element is not in the list
Block 2: element is the only element in the list
Block 3: element is the first element in a list with length bigger than 2
Block 4: element is the last element in a list with length bigger than 2
Block 3: element is an "inbetween" element in a list with length bigger than 3