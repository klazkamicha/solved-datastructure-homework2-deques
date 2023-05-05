Download Link: https://assignmentchef.com/product/solved-datastructure-homework2-deques
<br>
<h1>Deques</h1>

In class, you’ve learned in depth about Stacks and Queues, which are LIFO and FIFO data structures respectively. A Stack required you to add and remove from the same end of the data structure while a Queue required you to add and remove from opposite ends of the data structure.

For this assignment, you will be coding two implementations of a Deque. Deque is short for ”doubleended queue”, and it’s a data structure that allows for efficient adding and removing from both ends of the data structure.

The first implementation is backed by a Doubly-Linked List, and the second implementation is backed by a circular array.

<h2>LinkedDeque</h2>

As you will recall from when we learned about LinkedLists, in order to efficiently add/remove from both the front and back in <em>O</em>(1) time, we need a Doubly-Linked List (DLL) with a head and tail pointer. Thus, you will be implementing 4 methods for a DLL which are described in the javadocs of LinkedDeque.java.

<h2>ArrayDeque</h2>

The backing array in your ArrayDeque implementation must behave circularly. By this, we mean that your front and back variables should wrap around the beginning and end of the array as you add and remove to maintain <em>O</em>(1) efficiency while taking advantage of all the empty space in the array. There is a helper method to help you with the math part of this circular logic near the bottom of the ArrayQueue.java file called mod(int index, int modulo), so be sure to look at that as well.

<strong>IMPORTANT: </strong>Your front variable should represent the index holding the first element of the deque.

Your back variable should represent the index after the last element of the deque (and therefore the index to add to when at the back). <strong>Failure to follow this convention will result in loss of major points. </strong>The examples below demonstrate what the deque should look like at various states.

In the example below, the deque begins empty (initial state). When adding to the front here, the front wraps around to the back.

In the example below, adding to the back causes the back to wrap around to the front.

In the example below, adding another element causes the deque to resize since no more space is available, so the array capacity is doubled, front is reset to 0, and back is reset to the new size.

In the example below, the last element of the deque is removed, so the front/back are reset to their initial positions.

In the example below, the front/back wraps around depending on which end is removed from.