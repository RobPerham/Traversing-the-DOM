Let’s recap the parent and children relationship in the DOM hierarchy. A parent node is any node that is a direct ancestor of another node. A child node is a direct descendant of another node, called the parent node.

These relationships follow the nested structure of the HTML code. Elements nested within one HTML element are children of that parent element.

Each element has a .parentNode and .children property. The .parentNode property returns the parent of the specified element in the DOM hierarchy. Note that the document element is the root node so its .parentNode property will return null. The .children property returns an array of the specified element’s children. If the element does not have any children, it will return null.

<ul id='groceries'>
  <li id='must-have'>Toilet Paper</li>
  <li>Apples</li>
  <li>Chocolate</li>
  <li>Dumplings</li>
</ul>

In the HTML code above, we have an <ul> element with the ID of groceries with four <li> elements inside.

let parentElement = document.getElementById('must-have').parentNode; // returns <ul> element
let childElements = document.getElementById('groceries').children; // returns an array of <li> elements

Here, the parentElement variable stores the .parentNode of the <li> element with the ID of must-have, which will be the <ul> element with the ID of groceries. The childElements variable is set to the children of the <ul> element with the ID of groceries, which will be an array of four <li> elements.
