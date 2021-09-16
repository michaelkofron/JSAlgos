# Analyzing the performance of arrays and objects - the Big O of specific objects

```javascript

let instructor = {
	firstName: "Michael",
	isTeacher: true,
	favoriteNumbers: [1, 2, 3, 4]
}

```
Unordered, key value pairs

## Objects - When to use objects
- When you don't need order
- When you need fast access / insertion + removal

Objects are **O(1)** for insertion, removal, and access. They are **O(n)** for searching. So changing, updating, and removal are all extremely fast. There is no beginning or end of the object, we use keys instead.

"Searching" refers to finding something by a value. Accessing something by key is Big O constant.

## Big O Object Methods
- Object.keys - O(n)
- Object.values - O(n)
- Object.entries - O(n)
- hasOwnProperty - O(1)

For example, Object.keys goes through the object and places the keys into an array. The larger the array the more time it will take to do so for a complexity of **O(n)**

Since we can access a value in constant time we can also find if a property exists in constant time with hasOwnProperty

## Arrays - Ordered lists







