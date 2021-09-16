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

```javascript
let names = ["michael", "tom", "geek"]
```
## When to use arrays
- when we need order (not the only ordered structure, but the only we get for free)
- when we need fast access / insertion

- insertion - **big O depends**
- removal - **big O depends**
- searching - **O(n)**
- access - **O(1)**

```javascript
names[1]
```
this is constant, index 1 is like a "short cut". It doesn't matter how long the array is.

### insertion
- inserting to the end - **O(1)**
- inserting to the beginning - **O(n)** - this is because we have to now reindex every single item in the array

### removal
- **O(n)** because we also have to reindex every other item

## Big O of Array Methods

Most array methods are O(n). Any function that loops is obviously O(n)

Sort is O(n * log N) - We will learn about this later



