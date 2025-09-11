## What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Answer: Using getElementById(), we get a single element designated by the id. Contrarily, using getElementsByClassName(), we get all the elements addressed by the same class name.

querySelector() finds and returns the first single element of our interest. But, querySelectorAll() returns all the elements of our interest as a static NodeList. As a result, we need to use a loop (e.g., for loop) to access the NodeList returned by the querySelectorAll().
       
## How do you create and insert a new element into the DOM?
Answer: Firstly, we need to get the parent node using parentNode property. Then, we will create a new element using createElement() method. We can assign a class name to this new element using className property. For Example, using following code, we have created a new <div> element and assigned new-history class to this newly created element to apply the required CSS styles.  

let newHistory = document.createElement('div');
newHistory.className = 'new-history';

Finally, we need to add this element to its parent node using appendChild() method.  

## What is Event Bubbling and how does it work?
Answer: Event Bubbling is a DOM event propagation process. It is the later phase after Event Capturing.

Event Bubbling is a process which starts when an event is triggered on a child element and then it propagates upward automatically through its parent and ancestor elements until it reaches the root (<html>) of the DOM tree.

## What is Event Delegation in JavaScript? Why is it useful?
Answer: Event Delegation is another powerful and efficient event handling mechanism where we add an event listener to a parent node instead of adding an event listener to each of the child nodes separately.

Event Delegation helps to handle events triggered by all its child node, even though, the child may have been added dynamically later. Using less number of event listers, event delegation ensures optimized and cleaner code.

## What is the difference between preventDefault() and stopPropagation() methods?
Answer: The preventDefault() method prevents occuring the default action of an event. It impacts the default behavior of an event if its cancellable.

The stopPropagation() method just stops an event from bubbling up to its parent and ancestor nodes.    
