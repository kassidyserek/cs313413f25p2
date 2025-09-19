COMP 313/413 Project 2 Report Template

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		the same tests pass so there's no difference

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			it removes the element at index 5

		list.remove(Integer.valueOf(5)); // what does this one do?

			it removes the first value 5 that appears

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			it removes the first 77 !!!!

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.

	SIZE 10
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:   20   16   17   15   15   15  ... (fill these in in ms)
        testLinkedListAddRemove:   3    0    1    0    0    0
		testArrayListAccess:       0    0    0    0    0    0
        testLinkedListAccess:      1    0    0    0    0    0

	SIZE 100
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:   17   16   17   16   16   16  ... (fill these in in ms)
        testLinkedListAddRemove:   1    1    1    0    0    1 
		testArrayListAccess:       0    0    0    0    0    0 
        testLinkedListAccess:      1    1    2    1    1    1 

	SIZE 1000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:   33   23   24   23   24   26  ... (fill these in in ms)
        testLinkedListAddRemove:   0    0    0    0    0    1
		testArrayListAccess:       0    0    0    0    0    0
        testLinkedListAccess:     26   26   25   24   25   27

	SIZE 10000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:   124  124  112  110  126  118  ... (fill these in in ms)
        testLinkedListAddRemove:   0    3    0    0    0    0
		testArrayListAccess:       0    0    0    0    0    0
        testLinkedListAccess:     292  297  290  298  289  289

	listAccess - which type of List is better to use, and why?

		ArrayList since it's constant time, O(1), rather than linear time, O(n)

	listAddRemove - which type of List is better to use, and why?

		LinkedList is better when in the middle but ArrayList is faster for at the end