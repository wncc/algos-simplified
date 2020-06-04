## Fast Multiplication Using Divide And Conquer Algorithms

Hello there, this time we will be looking at divide and conquer algorithms and their application in multiplication of numbers, matrices and polynomials. You might be wondering, why bother with such sophisticated algorithms for something as trivial as multiplication? Well the naive multiplication algorithms that we study in school for multiplying numbers is slow. Given two numbers of digit count n the trivial multiplication algorithm takes roughly n^2 steps. Can we do better?

It turns out we can. The main idea is to reduce the problem into smaller subproblems, solve these problems and combine the result. This is similar to Merge Sort and this way of solving problems is termed as divide and conquer. Let's apply Divide and Conquer for integer multiplication using Karatsuba.

## Karatsuba's Algorithm

Karatsuba's algorithm basically splits your number into two numbers at it's midpoint. For instance 1423 can be written as 100(14) + (23). We can express the product of 1423 with another number in terms of the products of the smaller terms (14, 23) with the smaller terms of the other number. We will then combine these terms to get the final resultant product.

This [video](https://www.youtube.com/watch?v=JCbZayFr9RE) provides a simple and gentle introduction to Karatsuba. 
I personally found [these](http://web.stanford.edu/class/cs161/Lectures/Lecture1/Lecture1-compressed.pdf) slides from the CS 161 Algorithms course of Stanford very easy to read and englightening. Karatsuba is explained in a very simple and nice manner here with more details such as the time complexity of the algorithm. You might want to start from slide number 38 as the beginning focuses on their course details.

Let us now try to multiply matrices more quickly using divide and conquer.

## Strassen's Algorithm

The main insight in Karatsuba's algorithm was that by dividing the problem into subproblems of half the size we could reduce the number of operations. You should notice and prove that if we do four multiplications (or solve four subproblems) in total for combining the subproblems, we still end up with a quadratic algorithm for multiplication. Karatsuba gave us benefits because we could bring this count of four down to three. Maybe we can do something similar for square matrices?

Turns out we can. The main idea is to consider block matrices in the square matrices. Breaking down the multiplication into multiplications of the block matrices (total of 8) still results in a cubic algorithm for multiplying which is the same as the naive multiplication algorithm. However again we can clever bring this number down to 7 leading to a speed up.

Watch this [video](https://www.youtube.com/watch?v=ORrM-aSNZUs) by Stanford Algorithms which explains the math along with the algorithm behind Strassen's Algorithm.
[These](https://stanford.edu/~rezab/classes/cme323/S16/notes/Lecture03/cme323_lec3.pdf) notes from Stanford explain the same textually with some more details.

Let's now go into Polynomials!

## Fast Fourier Transform

(Note: This is a very advanced algorithm so we won't be able to make you understand this in 15 mins!)

Multiplying two polynomials of degree n takes n^2 steps naively when we loop over the polynomial coefficients. As you might have guessed there is a better way than this by using divide and conquer. Fourier comes to our rescue and using the discrete fourier transform we can actually make the multiplication happen in nlogn. The idea here is far more subtle and involves using complex numbers to split the problem into subproblems. Once we can take the discrete fourier transform of our sequence of coefficients quickly we can use the DFT for multiplying polynomials. 

These three videos by Gaurav Sen explain FFT in a very nice and complete manner: [FFT Part 1](https://www.youtube.com/watch?v=Xwu6rq41nE8), [FFT Part 2](https://www.youtube.com/watch?v=Y4R_I9NjlLI) and [FFT Part 3](https://www.youtube.com/watch?v=O87Z-v0GEEw).

You can also refer to [this](https://cp-algorithms.com/algebra/fft.html) article on CP Algorithms that provides a more detailed written implementation along with the applicaion of FFT for multiplying polynomials. [This](https://codeforces.com/blog/entry/43499) link on codeforces also explains it very well. This algorithm is very useful for solving hard problems as many questions can be rephrased in terms of polynomial multiplciations. You can refer to [this](https://github.com/geekpradd/Fast-Fourier-Transform) repository for the code for FFT in C++ along with the solution to one problem of Codechef Long that can be solved using FFT.


## Practice!

1. We talked about using Karatsuba for integer multiplication. Can you modify it for Polynomials? This will be slower than FFT but it will be far far simpler right?
2. These two codechef problems, [REBTET](https://discuss.codechef.com/t/rebtet-editorial/11880) and [BINOFEV](https://www.codechef.com/DEC19A/problems/BINOFEV/) can be solved with FFT. You should try to find the polynomials that can be used to solve these problems and then try to use FFT to multiply the polynomials and solve the problem.
3. [This](https://codeforces.com/contest/528/problem/D) is a relatively simpler codeforces problem which can be solved with FFT.
4. Understanding Strassen's algorithm is one thing, implementing it is another. Implement Strassen's algorithm in C++/Python and compare it's performance with the naive matrix multiplication algorithm.

That's it for today. Hope you all had fun!
