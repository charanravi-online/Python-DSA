You're probably here to learn some data structures and algo using python.\
Don't really want to waste your time here, so let's get straight to it.

# Contents
1. [Why DSA?](#Why-DSA?)
2. [Why Python?](#Why-Python?)
3. [Asymptotic?](#Asymptotic?)
4. [Big O Notation](#Big-O-Notation)
5. [Theta Notation](#Theta-Notation)

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
   
