# Limesharp Developer Test

Please, **don't fork this repo**, clone it or download it locally and then commit changes after each task into a new repo of your own, and send us the link. We will get back to you shortly. 

Languages accepted: Javascript or PHP. 

### Task 1: 
Make this work (repeat 3 times the contents of an array):
```javascript
repeat([1,2,3]) //[1,2,3,1,2,3,1,2,3]
```
Your solution:

```
function repeat(values){

    return Array(3).fill(values).flat();
}

repeat([1,2,3]);

// Repeat the array 3 times, fill the function parameter with the values passed and then flatten it to an array.
```

###### If we type in our console your function and repeat([1,2,3]) then the result should be [1,2,3,1,2,3,1,2,3] 

### Task 2:
Make this work (no vowels, lowercase except the first letter):
```javascript
reformat("liMeSHArp DeveLoper TEST") //Lmshrp dvlpr tst
```
Your solution:

```
function reformat(str) {

    const msg =  str.replace(/[aeiou]/gi,"").toLowerCase();
    return msg.charAt(0).toUpperCase()+ msg.slice(1);

}

reformat('liMeSHArp DeveLoper TEST');

// Use regex to find the vowels and remove them. Transform the string to lower case, find the first character of the string and transform it to upper case and then append it to the remaining string.
```

###### If we type in our console your function and reformat("liMeSHArp DeveLoper TEST") then the result should be Lmshrp dvlpr tst


### Task 3 (optional, for bonus points):
Make this work (without using any built in functions, only a `for` loop, return the next binary number in a string or as an array)
```javascript
next_binary_number([1,0]) // [1,1]

// possible test cases:
// [1,0] => [1,1]
// [1,1] => [1,0,0]
// [1,1,0] => [1,1,1]
// .......
// [1,0,0,0,0,0,0,0,0,1] => [1,0,0,0,0,0,0,0,1,0]
```
Your solution:

```
This test proved very challenging and fun but I could not solve this in time for the deadline. I learned a lot about binary numbers and bitwise operators in the process of researching !

Among other attempts the closest one I attempted was to take the binary value, turn it to a decimal with ES6's binary literal, iterate it once and then turn it back to a binary number. I could not complete it without using built in functions such as .toString(2).

```

###### If we type in our console your function and next_binary_number([1,0,0,0,0,0,0,0,0,1]) then the result should look like 1,0,0,0,0,0,0,0,1,0 (or as an array).

---

If you get invited to the first interview read the "What to expect.md" file.