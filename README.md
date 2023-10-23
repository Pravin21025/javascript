<!DOCTYPE html>
<html>
<head>
</head>
<body>
    <ul id="itemList">
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </ul>

    <script>
        // Get the parent element
        var parentElement = document.getElementById('itemList');

        // Create a new text node with "Hello World"
        var textNode = document.createTextNode("Hello World");

        // Create a new list item
        var newItem = document.createElement("li");

        // Append the text node to the new list item
        newItem.appendChild(textNode);

        // Append the new list item before the existing list item (Item Lister)
        parentElement.insertBefore(newItem, parentElement.firstElementChild);

        // Create another text node with "Hello World"
        var textNode2 = document.createTextNode("Hello World");

        // Create a new list item
        var newItem2 = document.createElement("li");

        // Append the text node to the new list item
        newItem2.appendChild(textNode2);

        // Append the new list item before the second list item (Item 1)
        parentElement.insertBefore(newItem2, parentElement.children[1]);
    </script>
</body>
</html>
