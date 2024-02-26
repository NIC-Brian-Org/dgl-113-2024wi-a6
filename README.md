# DGL 113 2024WI Assignment #6

Preview the docs/index.html file with a web browser to get a
general idea about the webpage layout and its functionality,
then complete the following tasks.

Create a new file in the `docs` folder called `app.js`.

At the top of the `docs/app.js` file, add the `use strict` directive:

```javascript
'use strict';
```

Add a `<script>` element to the `index.html` file to include the `app.js` script.
Place the `<script>` element just before the closing `</body>` tag just like
the script element that is used to include the `main.js` script.

Make a copy of the `OrderItem` class from Assignment #5.

Add a new method to the class `tr(d)` which returns a `tr` DOM element
for document `d`. The `tr` element you return must have 4 cells:

- the quantitity
- the size
- the description
- a "Delete" button

Create a new class `Order` as follows:

The class should maintain an array of `OrderItem` objects.

The class should have `add(item)` method that adds an item to the order.
Here, `item` is expected to be an `OrderItem` object.

The class should also have a `delete(index)` method that deletes an item
from the order at index position `index`.

The class should have a method `tbody(d)` which returns a `tbody` DOM element
for document `d`. The `tbody` element you return must have a `tr` DOM element
for each of the items in the order. You can the `tr(d)` method of the `OrderItem`
class described above to help with this.

The class should also have a `cost()` method which returns the total cost of the
entire order. You can use the existing `cost()` method from Assignment #5
to get the cost of the individual `OrderItem` objects.

Remember that:

- Short, Tall, Grande, and Venti coffees cost 2.99, 3.19, 3.49 and 3.99 respectively, and
- Short, Tall, Grande, and Venti teas cost 2.85, 3.05, 3.25, and 3.50 respectively.

NOTE: Only modify the `docs/app.js` and `docs/index.html` files.
Do not make changes to any other files.
