# JS_Array_Methods

We can use tinytest or simpletest to test our code.

Tiniest JavaScript unit testing library
This is an in-browser JavaScript library I've been using for years. It's so small and simple that it never occured to me to open source it until I saw all the overly complicated alternatives that are out there.

Let's say you have a function in adder.js:

function add(a, b) {
  return a + b;
}
Create a test page called adder-test.html (you can name it anything). This includes your code under test, tinytest.js and defines your tests:

<script src="tinytest.js"></script>
<script src="adder.js"></script>
<script>
 tests({

   'adds numbers': function() {
     eq(6, add(2, 4));
     eq(6.4, add(2.4, 4));
   },

   'subtracts numbers': function() {
     eq(-2, add(2, -4)); 
   },

 });
</script>
Open the page in your browser. Green is good. Red is bad. If it's red, look in the JavaScript console for messages.

That's it!

Follow the same process that we followed in the testing series for these array methods on your own. I recommend doing them in the order they appear below.

Verify your answers by comparing the behavior of your code against the native equivalents. After verifying, compare your code against solutions from other students.

Finally, before you continue, post your code as well so that others can learn from your approach.



Array.prototype.find

Array.prototype.findIndex

Array.prototype.every

Array.prototype.some

Array.prototype.reduceRight

Array.prototype.concat

Array.prototype.indexOf

Array.prototype.lastIndexOf

Array.prototype.includes

Array.prototype.slice

Array.prototype.join

Array.prototype.push

Array.prototype.pop

Array.prototype.shift

Array.prototype.unshift

Array.prototype.fill

Array.prototype.reverse

Array.prototype.copyWithin

Array.prototype.sort

Array.prototype.splice

