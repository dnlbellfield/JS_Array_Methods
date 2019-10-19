# JS_Array_Methods
Array Methods
we will use tinytest or simpletest to test out code.
Tiniest JavaScript unit testing library
This is an in-browser JavaScript library I've been using for years. It's so small and simple that it never occured to me to open source it until I saw all the overly complicated alternatives that are out there.

If you're looking for a JavaScript library full of features or install guides that say things like grunt, npm or bower, you've come to the wrong place. Sorry, this probably isn't for you. Move along now.

If you're looking for a quick way to unit-test a JavaScript function/object in a web-page and don't want to get bogged down in frameworks, you've come to the right place. Take a seat... no scratch that, you'll have everything you need in a few seconds so you may as well remain standing.

Download tinytest.js
Example
10 second tutorial
Download tinytest.js and put it somewhere in your web directory.

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

Don't believe me? Here's the source and result.

What else?
If your tests fail, you'll get stack traces:



Function reference
// Force a failure
fail(reason);

// Assert expression is truthy (fail with reason)
assert(expression, reason);

// Assert expected == actual
assertEquals(expected, actual)
eq(expected, actual) // Alias for assertEquals

// Assert expected === actual
assertStrictEquals(expected, actual)
Errm that's it. Now stop wasting time - go test that function.

But, but, but. What about feature X?
It probably doesn't have it. If you need that, you'll probably find it in one of the many more sophisticated frameworks out there. A more detailed discussion can be found here.

Projects using TinyTest
Filtrex - A simple, safe, JavaScript Filter Expression compiler (Tests) (Results)
Other stuff
I also have TinyTest for C that follows similar principles of simplicity.

Now check out my other GitHub projects and follow @joewalnes on that Twitter thing.


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
