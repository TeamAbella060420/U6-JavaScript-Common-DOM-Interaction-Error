# U6-JavaScript-Common-DOM-Interaction-Error
 
# Common DOM Interaction Errors
When selecting DOM elements and adding event listeners to elements, several common errors may occur. In this step, you’ll find examples of errors to check for while practicing your newly learned skills. Then you’ll find a few ways you can locate and prevent these errors.

# Types of Errors:

1. Misspelled class names - document.querySelector(‘.tablelist’) The above snippet would return null if the actual class name of the desired item was tableList. The names must match in spelling and case for the correct element to be selected.

2. Improper Selectors - When using a method such as getElementById(), a developer may accidentally pass it a class instead of an id. In this case, once again, no element will be selected. Some selectors return a single element, while others return a collection of elements.

Ensure that you have selected an individual item. document.querySelectorAll() returns a collection. You may loop through a collection to add event listeners, but you can not place a listener on the collection itself.

# Preventing & Finding Errors:

Here are a few ways you can stop DOM errors in their tracks and get your apps working.

1. Double Check - Always check that the method and its parameters are correct before running.
2. Console.log() - Selecting DOM elements is a great opportunity to use console.log() for checking values. You can console.log a variable that stores a selected DOM node to test if the correct value was selected. Adding a console.log statement inside an event listener allows you to check if the listener is working and check values within the handler function if needed.

# Code Validation

Sometimes, the error comes from somewhere else in your JavaScript and the code ends before your selection. There are tools called linters and validators that check for errors we miss, like missing closing brackets. Some of these tools are available as plug ins to your text editor while others are browser based. Make sure to use a linter or code validator to check for errors we all miss, like missing closing brackets.