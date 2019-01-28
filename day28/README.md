![cover](./cover.png)

# Day 28 - Search and Sort Algorithms Part A: the Linear Search

It's almost a month sincec we starated this initiative and we did questions on Strings, Arrays, Recursion and Misc. Also, in some questions, we tried to solve the question in best possible runtime, which improved our concepts of time complexity. Now, to make our code more efficient, it's highly essential that we know some frequently used searching and sorting algorithms and apply them in the code accordingly whenever required.

So this week we will be be focusing on various searching and sortinig algorithms. Today's Algorithm -- Linear Search

## Question

Write a program to implement linear search, to find the index of a given element in a given array

**Example**

```
input: arr = [1, 2, 3, 4, 5], num = 2
output: 1 (index of found element)

input: arr = [1, 2, 3, 4, 5], num = 7
output: undefined
```

![ques](./ques.png)

## Solution

### [JavaScript Implementation](./JavaScript/linear.js)

```js
function linearSearch (arr, n) {
    for (let i=0; i<arr.length; i++) 
        if (arr[i] === n)
            return i;

    return undefined;
}

console.log (linearSearch ([1, 2, 3, 4, 5], 2));
console.log (linearSearch ([1, 2, 3, 4, 5], 7));
```