

### **Task Title: “Interactive Web Page with DOM Manipulation”**

#### **Objective**

Use basic JavaScript DOM manipulation techniques to make a static HTML page interactive.
Students will create a mini webpage that responds to user actions — changing text, styles, creating/removing elements and handling events.



### **Instructions**

Create a simple webpage named `dom_task.html` and link a JavaScript file named `script.js`.

Your webpage should include:

```html
<h2 id="heading">Welcome to My Page!</h2>
<p id="text">Click the buttons below to interact with this page.</p>
<div id="container"></div>

<button id="changeTextBtn">Change Text</button>
<button id="changeStyleBtn">Change Style</button>
<button id="addItemBtn">Add Item</button>
<button id="removeItemBtn">Remove Item</button>
<button id="fetchDataBtn">Fetch Data</button>

<ul id="list"></ul>
```



### **Tasks to Complete in `script.js`**

1. **Change Text Content**

   * When the “Change Text” button is clicked, change the paragraph text (`#text`) to something new.

2. **Change Style**

   * When the “Change Style” button is clicked, change the background color and text color of the heading (`#heading`).

3. **Add a New List Item**

   * When “Add Item” is clicked, add a new `<li>` element to the list with text like “New Item added!”

4. **Remove a List Item**

   * When “Remove Item” is clicked, remove the *last* list item (if any).
