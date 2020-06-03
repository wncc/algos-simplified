## Fast Multiplication Using Divide And Conquer Algorithms

Hello there, this time we will be looking at divide and conquer algorithms and their application in multiplication of numbers, matrices and polynomials. You might be wondering, why bother with such sophisticated algorithms for something as trivial as multiplication? Well the naive multiplication algorithms that we study in school such as the one algorithm drilled into our minds from Class 1 onwards for multiplying numbers is well slow. Given two numbers of digit count n the trivial multiplication algorithm takes roughly n^2 steps. Can we do better?

It turns out we can. The main idea is to reduce the problem into smaller subproblems, solve these problems and combine the result. This is similar to Merge Sort and this way of solving problems is termed as divide and conquer. Let's apply Divide and Conquer for integer multiplication using Karatsuba.

## Karatsuba's Algorithm

Karatsuba's algorithm basically splits your number into two numbers at it's midpoint. For instance 1423 can be written as 100*(14) + (23). We can express the product of 1423 with another number in terms of the products of the smaller terms (14, 23) with the smaller terms of the other number. We will then combine these terms to get the final resultant product.

I personally found these slides from the CS 161 Algorithms course of Stanford very easy to read and englightening. Karatsuba is explained in a very simple and nice manner [here](http://web.stanford.edu/class/cs161/Lectures/Lecture1/Lecture1-compressed.pdf). You might want to start from slide number 38 as the beginning focuses on their course logistics.
