This is my personal notes for data structures and algorithms.\
Making this publicly available just in case anyone else finds it useful.\

# Contents
1. [Why DSA?](#Why-DSA?)
2. [Why Python?](#Why-Python?)
3. [Asymptotic?](#Asymptotic?)
4. [Big O Notation](#Big-O-Notation)
5. [Theta Notation](#Theta-Notation)
6. [Properties of Asymptotic Notations](#Properties-of-Asymptotic-Notation)
7. [Worst, Average and Best case time complexities](#Worst-Average-Best-Case-Time-Complexities)


## Why-DSA?
1. To make yourself a better developer.\
(you could save a lot of your CPU cycles if your code is optimised, and on a large scale, that's going to save your organisation a lot of money, which is why they would hire someone who is well versed)
2. To get hired lol.
3. Competitive coding, If you're one of the few people who sees coding as a fun, competitive and an interesting activity. 



## Why-Python?
1. Let's just be honest here, you chose python because it's pretty neat and easy to understand didn't you?\
   Yeah it is pretty easy to read and beginner friendly.
2. Don't stress too much about the language.
3. Python, Java or C++? Relax and go with whatever you feel comfortable with. 


## Asymptotic?
1. If you'd want any code to be run in least time possible (not really caring about the optimisations), you could use a super fast system with all the high end specs.\
   Chances are, it will run faster in that than a potato PC. But, this becomes variable. How your code runs in certain environments changes depending on the environment,\
   and this only makes things more difficult for us to calculate the efficiency of our code.\
   (When you use a different programming language like C, it is a compiled language and could take less exeuction time as compared to Python which is an interpreted language.)
3. This is why we use Asymptotic Analysis. We don't even have to write the entire code to begin our analysis. All we need is pseudo code or the algorithm ready.\
   We would use this to tell how efficient our piece of code is depending on the input we give.
4. To summarise,
   - No dependency on machine, programming language, etc.
   - We do not have to implement all ideas and algorithms.
   - Asymptotic analysis is about measuring order of growth in terms of input size.
  
5. Example : "add example here"

## Big-O-Notation
1. To put it simply, imageine you're comparing ways to sort a list of numbers.\
   The big O Notation helps you understand how these methods perform as the list gets longer.

2. Example: Let's say you have a list of 10 numbers. One method might take 10 steps to sort it while another might take 100 steps.\
   With Big O Notation, we ignore exact numbers and focus on how these methods behave as the list grows infinitely long.

3. In summary, Big O Notation tells us how an algorithm's performance changes as the amount of data it's working on changes,\
   using simple terms like "linear" or "quadratic" to describe this behavior.

## Theta-Notation
1. Okay, so imagine you're on an roadtrip, and you want to know how long it would take. It could take around\
   4 to 6 hours, depending on traffic and road conditions.\

   - The Big O Notation would be saying "At most it'll take 6 hours".\
   Observe that it is the worst case scenario.

   - The Theta Notation (Θ) on the other hand would say "It'll take between 4 ot 6 hours."\
   Observe that it gives a more precise range , showing both the minimum and maximum times.

2. So, while Big O gives you the upper limit, Theta gives you a range that's closer to reality, showing both the best and worst-case scenarios.

## Omega-Notation
1. Just as Big O represents asymptotic upper bound of a function, Omega Notation (Ω) provides asymtotic lower bound of a function.
2. What this means is it gives the best case scenario of a function.
3. To understand this better, imagine you're planning another road trip, and this time you know it's going to take at least 4 hours,\
   but it could take longer depending on the traffic and road conditions.\
   - Big O Notation would be saying, "At most it'll take 6 hours."\
     It gives you the maximum time you'll spend on the road.
   - Theta Notation would say "It'll take between 4 to 6 hours."\
     It gives you a range, showing both the minimum and maximum time it could take.
   - Omega Notation would say, "It'll take at least 4 hours."\
     It gives you the minimum time you'll spend on the road.
4. So, Omgega notation focuses on the lower limit, giving you an idea of the best case scenario.\
   It is also the least used notation among these three.


## Properties-of-Asymptotic-Notation
1. ### General Properties
   ``` If f(n) is O(g(n)) and k is constant then k*f(n) is also O(g(n))```\
   Let's look at this with an example,\
   f(n) = 2n²+5 is O(n²)\
   then 7*f(n) = 7(2n²+5) = 14n²+35 is also O(n²).\
   Similarly, this property satisfies both Θ and Ω notation. 

2. ### Transitive Properties
   ``` If g(n) is O(h(n)) and f(n) is O(g(n)) then f(n) = O(h(n)) ```\
   Let's look at this with an example,\
   Example: if f(n) = n, g(n) = n² and h(n)=n³\
   n is O(n²) and n² is O(n³)\
   then n is O(n³)\
   Similarly, this property satisfies both Θ and Ω notation.
   
4. ### Reflexive Properties
   ```given f(n), then f(n) = O(f(n))```\
   Let's look at this with an example,\
   consider two funcitons\
   f(n) = n^2 and f(n) = n^3
   we can say that\
   f(n) = O(n^2) and g(n) = O(n^3)
   that is because f(n) grows at a equal rate or slower than n^2.\
   this is the same with g(n) as well.
   This demonstrates the reflexive property in action,\
   showing that a function can be bound above by different\
   functions while still maintaining its growth rate.

5. ### Summetric Properties
   ```If f(n) is Θ(g(n)) then g(n) is Θ(f(n))```\
   Let's look at this with an example.\
   there are two funcions\
   f(x) = x^2 & g(x) = 2x\
   as x becomes very large: f(x) grows faster than g(x)\
   as x becomes very small: g(x) grows faster than f(x)\
   SO, the symmetric property in this case means that when one function is faster that the other as x gets large, the situation flips when x gets small.\
   It's like a balance where one funciton dominates in one direction and another funtion in the opposite direction.

6. ### Transpose Symmetric Properties
   ``` If f(n) is O(g(n)) then g(n) is Ω (f(n)) ```\
   Let's look at this with an example,\
   consider two funcitons\
   f(x) = x^3 & g(x) = 4x^2\
   If f(x) grows faster than g(x) as x approaches positive infinity, then f(-x) grows faster than g(-x) as x approaches negative infinity.\
   This property shows that if one function grows faster than another function for large positive inputs, the same relationship holds when you switch to large negative inputs by negating x.

7. ### Other Properties
   Well there are a few more properties but I guess it's something that can be easily googled (if you feel the need to that is).\
   The reason I'm skipping it is becaues it is pretty boring and it is quite simple. That could be a homework of sorts.

## Worst-Average-Best-Case-Time-Complexities
We'll look at a linear search example and try to get the Worst, Average and Best case time complexities.
```
def search(arr, x):

	for i in range(len(arr)):
                     
		if arr[i] == x:
			return i

	return -1
```
### Worst Case (Commonly used)
In the worst case we calculate the upper bound on running time of an algorithm.
The code above takes an array and the element to be searched form the array. \
The worst case is when the element to be searched is not present in the array. When x is not present, the search() compares x with all the elements of the array one by one.\
Therefore the worst case for a linear search could be O(N) where N is the number of elemets in the array.

### Average Case (Not so commonly used)
Here we are just referring to estimation of the performance of an algorithm based on the average input it is likely to encounter, which involves calculating the average time complexity or space complexity over all possible inputs of a given size.
1. Identify the possible scenarios: In a linear search the target could be at any position in the array, including first, last or any intermediate position.
2. Assign probabilities: If the list has 10 elements, assume that the probability becomes 1/n where n is the element in the list/array.
3. Calculate the average time: The average case time complexity is calculated by taking the weighted sum of the time taken in each scenario where the weight is the probability of that scenario occuring.

### Best Case (Why even?)
So, the best case occurs when the element we are looking for is in the first location. Which would mean that the number of operations in the best case is constant, and doesn't depend on N, making the complexity O(1).\
Which is also why this is not used that much, since it does't really add all that value.

### Note
We mostly do the worst case where we guarantee an upper bound on the running time of an algorithm which is useful information.\
We rarely do average case since it is not easy to do in most of the practical cases and we must know the mathematical distribution of all possible inputs.\
Coming to best case, guaranteeing a lower bound doesn't help much if the worst case takes years to run.


