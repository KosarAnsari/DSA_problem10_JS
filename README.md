# 🧠Day 10 - 21 Day DSA Challenge

## Topic: Sorting & Sorted Array Check using Recursion

### 📚 **What I Learned**
- How to check if an array is sorted.
- Recursive approach to sort an array.
- Swapping elements using JavaScript destructuring.
- How recursion can simplify array operations by breaking them into smaller steps.

---

##💡 **Code Implemented**

```javascript
let i = 0;
let j = 1;
let mynewList = [];
let myArray = [2, 3, 1, 4];

function isSorted(array) {
    for (let i = 0; i < array.length; i++) {
        if (array[i] > array[i + 1]) {
            return false;
        }
    }
    return true;
}

function sortCheck(array) {
    if (isSorted(array)) {
        mynewList = array;
        return;
    } else if (array[i] < array[j]) {
        i++;
        j++;
        sortCheck(array);
    } else {
        [array[i], array[j]] = [array[j], array[i]];
        i = 0;
        j = 1;
        sortCheck(array);
    }
}

sortCheck(myArray);
console.log(mynewList);


---

Steps in the Code

1. isSorted(array):

Checks if the array is sorted in ascending order.

Returns true if sorted, otherwise false.



2. sortCheck(array):

Uses recursion to compare elements.

If elements are not in order, swaps them and restarts checking.

Continues until the array is fully sorted.



3. Result:

The sorted array is stored in mynewList and printed in the console.





---

Example

Input:
[2, 3, 1, 4]

Output:
[1, 2, 3, 4]


---

☑️Key Takeaway

This challenge helped me gain a deeper understanding of recursion and sorting algorithms, and how we can implement sorting logic without using built-in functions.


---

#DSA #JavaScript #Recursion #ProblemSolving #Day10


