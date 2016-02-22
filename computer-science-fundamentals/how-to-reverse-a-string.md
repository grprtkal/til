# Reversing a string using recursion 

A recursive function calls itself. 

There are 4 important aspects of a recursive function: 

1. The function calling itself (recursion)
2. A base case which ends the recursion 
3. Modifying the arguments such that the arguments lead to the base case 
4. (Optional) A termination condition which cancels the recursion in case of a bad input or error

To reverse a string, we slice off everything in our string starting from the second letter (at index 1) and add the first character (at index 0) to the end. We keep doing this (recursively) until we only have one letter left as an argument in our recursion. 

```
function reverse(str) {
  if (str.length <= 1) { // base case
    return str;
  }
  reverseString = reverse(str.slice(1)) + str[0]; // modify our argument
  return reverseString; // recursion
}

reverse("hello");

```

Our stack would be as follows: 

```
1. reverse("ello") + h
2. reverse("llo") + e + h
3. reverse("lo") + l + e + h
4. reverse("o") + l + l + e + h
5. o + l + l + e + h
```
