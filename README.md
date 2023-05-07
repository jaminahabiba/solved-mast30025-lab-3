Download Link: https://assignmentchef.com/product/solved-mast30025-lab-3
<br>
MAST30025: Linear Statistical Models

Week 3 Lab

<ol>

 <li>Let <em>X </em>be a 10 × 5 matrix of full rank and let <em>H </em>= <em>X</em>(<em>X<sup>T</sup>X</em>)<sup>−1</sup><em>X<sup>T</sup></em>.</li>

</ol>

Find <em>tr</em>(<em>H</em>) and <em>r</em>(<em>H</em>).

<ol start="2">

 <li>Let</li>

</ol>

<em>.</em>

Let <em>z </em>= <strong>y</strong><em><sup>T</sup>A</em><strong>y</strong>. Write out <em>z </em>in full, then find <em><sub>∂</sub><u><sup>∂z</sup></u></em><strong><sub>y </sub></strong>directly <em>and </em>using the matrix formula.

<ol start="3">

 <li>Let <strong>y </strong>be a random vector with mean <em>µ</em>, and assume that</li>

</ol>

Var<em>y<sub>i </sub></em>= 4 and Cov(<em>y<sub>i</sub>,y<sub>j</sub></em>) = 0.

<ul>

 <li>Write down Var<strong>y</strong>.</li>

 <li>Let</li>

</ul>

and find Var<em>A</em><strong>y </strong>and E[<strong>y</strong><em><sup>T</sup>A</em><strong>y</strong>]

<ol start="4">

 <li>Prove corollaries 3.6 and 3.7 from the lectures.</li>

 <li>Let <strong>y</strong> be a normal random vector with mean and variance</li>

</ol>

<em>µ</em> and<em>.</em>

Let

<em> .</em>

<ul>

 <li>Find the distributions of <strong>y</strong><em><sup>T</sup>A</em><strong>y </strong>and <strong>y</strong><em><sup>T</sup>B</em><strong>y</strong>.</li>

 <li>Are <strong>y</strong><em><sup>T</sup>A</em><strong>y </strong>and <strong>y</strong><em><sup>T</sup>B</em><strong>y </strong>independent?</li>

 <li>What is the distribution of <strong>y</strong><em><sup>T</sup>A</em><strong>y </strong>+ <strong>y</strong><em><sup>T</sup>B</em><strong>y</strong>? 6. Let <em>y</em><sub>1</sub><em>,…,y<sub>n </sub></em>be an i.i.d. normal sample. Show that</li>

</ul>

and

are independent. (<em>Hint</em>: Express them as a random “vector” and quadratic form respectively.)

<h1>R exercises</h1>

The following are taken from Chapter 3 of spuRs (Introduction to Scientific Programming and Simulation Using R).

<ol>

 <li>Consider the function <em>y </em>= <em>f</em>(<em>x</em>) defined by</li>

</ol>

<table width="164">

 <tbody>

  <tr>

   <td width="39"><em>x</em></td>

   <td width="44">≤ 0</td>

   <td width="54">∈ (0<em>,</em>1]</td>

   <td width="27"><em>&gt; </em>1 √</td>

  </tr>

  <tr>

   <td width="39"><em>f</em>(<em>x</em>)</td>

   <td width="44">−<em>x</em><sup>3</sup></td>

   <td width="54"><em>x</em>2</td>

   <td width="27"><em>x</em></td>

  </tr>

 </tbody>

</table>

Supposing that you are given <em>x</em>, write an R expression for <em>y </em>using if statements.

Add your expression for <em>y </em>to the following program, then run it to plot the function <em>f</em>.

# input

x.values &lt;- seq(-2, 2, by = 0.1)

# for each x calculate y n &lt;- length(x.values) y.values &lt;- rep(0, n) for (i in 1:n) { x &lt;- x.values[i]

# your expression for y goes here y.values[i] &lt;- y

}

# output

plot(x.values, y.values, type = “l”)

Your plot should look like Figure 1. Do you think <em>f </em>has a derivative at 1? What about at 0?

<ol start="2">

 <li>Let. Write an R program to calculate <em>h</em>(<em>x,n</em>) using a for</li>

 <li>The function <em>h</em>(<em>x,n</em>) from Exercise 2 is the finite sum of a geometric sequence. It has the following explicit formula, for <em>x </em>6= 1,</li>

</ol>

<em>.</em>

Test your program from Exercise 2 against this formula using the following values

You should use the computer to calculate the formula rather than doing it yourself.

<ol start="4">

 <li>First write a program that achieves the same result as in Exercise 2 but using a while Then write a program that does this using vector operations (and no loops).</li>

</ol>

If it doesn’t already, make sure your program works for the case <em>x </em>= 1.

<ol start="5">

 <li>To rotate a vector (<em>x,y</em>)<em><sup>T </sup></em>anticlockwise by <em>θ </em>radians, you premultiply it by the matrix</li>

</ol>

<em>.</em>

Write a program in R that does this for you.

<ol start="6">

 <li>Given a vector x, calculate its geometric mean using both a for loop and vector operations. (The geometric mean of</li>

</ol>

You might also like to have a go at calculating the harmonic mean, (, and then check that if the <em>x<sub>i </sub></em>are all positive, the harmonic mean is always less than or equal to the geometric mean, which is always less than or equal to the arithmetic mean.

<ol start="7">

 <li>A room contains 100 toggle switches, originally all turned off. 100 people enter the room in turn.The first toggles every switch, the second toggles every second switch, the third every third switch, and so on, to the last person who toggles the last switch only.</li>

</ol>

At the end of this process, which switches are turned on?

x.values

Figure 1: The graph produced by Exercise 1.<img decoding="async" data-recalc-dims="1" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2022/04/463.png?w=980&amp;ssl=1" class="lazyload" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==">

 <noscript>

  <img decoding="async" src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2022/04/463.png?w=980&amp;ssl=1" data-recalc-dims="1">

 </noscript>