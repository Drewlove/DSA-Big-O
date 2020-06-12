1. What is the Big O for this?

1) O(1)
2) O(n)


2. Even or odd
O(1)

The function is basic arithmetic, which has a parameter that must be a single number, so the time complexity it takes to solve the problem is constant regardless of the size of the input. 


3. Are you here? 
O(n^2)

The function has two nested loops, and so run time complexity grows exponentially as either array increases in size. 

4. Doubler
O(n) 
The function has to traverse across every element of an array and perform a simple arithmetical operation on each element. Since it only traverses each element once, the time complexity is directly proportional to the size of the array, thus, O(n).

5. Naive Search 
O(n) 
The function traverses across an array. Even though it could be solved in a very short period of time if the first element in the array matches the item, Big O is only concerned with the most time consuming version of the function. As such, the matching element would be at the end of the array, which means the time it takes to find the matching element is directly proprotional to the length of the array. 

6. Creating Pairs
O(n^2)

The function has two nested loops, and so run time complexity grows exponentially as either array increases in size. 

7. The algorithm computes the fibonacci sequence of a given number. The runtime complexity is O(n) because it is directly proportional to the input as it will generate an array that is of equal length to the number passed into the function as its argument. 


8. An Efficient Search 
O(log(n))
The time complexity is proportional to the array size, but since the algorithm effectively divides the array into two arrays, and then searches whichever array contains the item, the time complexity is only logarithmically proportional, as opposed to being directly proportional as is the case with O(n)


9. Random element
O(1)

The function does a simple arithmetic operation, so regardless of array size, it will essentially require the same amount of time to complete the operation. 


10. What Am I? 
O(n)
The function determines if the argument is a prime number. 

The time complexity is O(n), because, in a worst case scenario, the function must perform an arithmetic operation on every whole number preceding the argument, beginning with 2 and incremeting by 1. So, since increasing the value of the argument has a directly proportional increase on the time complexity, the time complexity is O(n). 


12. Iterative Version

1. Counting Sheep
Time Complexity: O(n)
function countSheep(num) {
  let solution = "";
  let i = 0

  
  while (num > 0) {
    solution +=`${num}: Another sheep jumps over the fence. `;
    num--; 
  }
  
  return solution += `All sheep jumped over the fence.` 
}

2. Power Calculator
Time Complexity: O(n)
function powerCalculator(base, exponent){
  let product = base
  let i = 1; 
  
  while(i < exponent){
    product = product*base
    i++
  }
  
  return product
}


const result = powerCalculator(5, 3)
console.log(result)


3. Reverse String
Time Complexity: O(n)

function reverseString(string){
  let answer = ''
  let i = string.length
  
  while(i > 0){
    i--
    answer += string[i]

  }
  return answer
}


let string = 'hello'
const answer = reverseString(string)
console.log(
  answer
)


4. nth Triangular Number
Time Complexity: O(n)

function iterativeFunction(n){
  let list = [1, 3]
  let i = 0

  while(i < n){
    let nextDiff = list[i+1] - list[i]
    let nextNum = nextDiff + 1 + list[i+1]
    list.push(nextNum) 
    i++
  }
  
  return list[n]
}




5. String Splitter
Time Complexity: O(n)

function iterativeFunction(string, delimiter){
  let answer = []
  let subString = ''
  let i = 0
  
  while(i < string.length){
    if(string[i] === delimiter){
      answer.push(subString)
      subString = ''
      i++
    }
    subString += string[i]
    i++
  }  
  answer.push(subString)

  return answer
}




6. 

