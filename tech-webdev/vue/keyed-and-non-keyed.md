# Keyed vs non-keyed JS frameworks 

A framework can implement an update for a list of items in two ways:
1. It keeps an association between a list item and DOM node (keyed mode) 
2. It rearranges and reassigns DOM nodes as it sees fit (non-keyed)

*Keyed* implementations create an association between the domain data and a DOM element by assigning a 'key'. If data changes the DOM element with that key will be updated. As a consequence, inserting or deleting an element in the data array causes a corresponding change to the DOM.

*Non-keyed* implementations are allowed to reuse existing DOM elements. As a consequence, inserting or deleting an element in the data array might append after or delete the last table row and update the contents of all elements after the insertion or deletion index. This can perform better, but can cause problems if DOM state is modified externally.

Using CSS transitions or third-party frameworks in non-keyed mode often causes problems. This is because, e.g. removing a list item may instead remove the last item from the DOM node list, patching other items to display the correct values. This can cause problems when e.g. CSS transitions styles depend on removing the specific node.

Keyed frameworks also have a non-keyed mode, entered by assigning the list's array index as a key. From the framework's perspective handling only non-keyed updates makes DOM reconciliation much faster.
