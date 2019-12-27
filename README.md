# glas-data-programming-challenges

> Please complete the challenge outlined below.

Given the following relational object structure:

```
{
	id: "unique_id",
	parentId: "another_id"
}
```

Build a liked list, or "parent tree". 

# Example 1:

### Input:

```
[
	{
		id: "one",
		parentId: null
	},
	{
		id: "two",
		parentId: "one"
	},
	{
		id: "three",
		parentId: "two"
	},
	{
		id: "four",
		parentId: "two"
	}
] // the array of objects in any order
-1 // the depth to which to build the tree
```

### Output:

```
{
	one: {
		id: "one",
		parentId: null,
		children: ["two"]
	},
	two: {
		id: "twp",
		parentId: "one",
		children: ["three", "four"]
	},
	three: {
		id: "three",
		parentId: "two":
		children: []
	},
	four: {
		id: "four",
		parentId: "two",
		children: []
	}
}
```

# Description

The solution should be a function that takes two arguments:

* An array of objects in any order
* A depth parameter specifying to which depth the tree should be built


Given the following object structure:

![structure](./Challenge.jpg)


