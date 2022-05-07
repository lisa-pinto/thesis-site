---
author: Lisa
description: Common Factors and pretty tiles
date: "2022-04-24"
image: tiles.webp
tags:
- emoji
title: Common Factors and pretty tiles
math: true
---
# Traditional Tile inlay
Various locations.


## Introduction

Tiles are based on Patterns of smaller components fitting into a bigger space

{{< rawhtml >}}
<div style="display: flex; width:100%;padding-left:10%;align-items: center; ">
<div class="threecolumn">
<img src="/images/jones.jpg" style="width:100px;"> 
<br> William jones was the first recorded person to use the symbol pi for pi* 
</div>
<div class="threecolumn">
<img src="/images/euler.webp" style="width:100px;">
<br>In 1607, Leonard Euler, assigned e to the value 2.7182818284….
</div>
<div class="threecolumn">
<img src="/images/gauss.jpg" style="width:100px;">
<br>In 1755, Gauss first assigned the letter I to root of -1 
</div>
</div>   
{{< /rawhtml >}}               

If you take a rectangular space, only a certain number of full-sized tiles will be able to fit into it. 

Let’s take Two variables, A and B
(A has to be greater or equal to B)
Suppose you have the Numbers 39 and 15
15 fits two times into 39, and you still have 9 left over
 
Now you have the equation 
39 = 15(2) + 9
{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/15.png" style="width:400px;">
</div>
{{< /rawhtml >}}
 
This is called Euclid’s Division Lemma, which states that”
for every two numbers a and b, there will be a number q (that is the maximum times that b fits into a), and r (a little bit left over), so that
a = b(q) + 2

{{< rawhtml >}}
<div class="center">
<img src="/images/euclid.jpg" style="width:400px;">
</div>
{{< /rawhtml >}}


To understand more, play around with the exercise below

{{< rawhtml >}}
<div class="center">
<iframe 
        src="https://editor.p5js.org/lisa-pinto/full/W5iBROolh"
        style="border-style: none;width: 800px; height: 450px"
         >
</iframe>
</div">
{{< /rawhtml >}}

So far, we’ve been able to see how ,many times b fits into a. But can we find a number that fits into both b an a?
Euclid Developed a nifty trick that allows us to find out the largest tile that can fit an area.


Let’s Take The numbers 39 and 15 again
Since 15 is the smaller side, it is the largest possible tile size that can be used. 
We know that the biggest possible tile is 15, and you will have 9 remaining.

{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/15.png" style="width:400px;">
</div>
{{< /rawhtml >}}
 
Let’s try to break that remaining piece down. 
You can, divide the remaining space by 9, but 9 does not fit into 15, so you will still have 6 remaining
{{< rawhtml >}} -->
 <div class="center">
<img src="/images/tiles/9.png" style="width:400px;">
</div> -->
{{< /rawhtml >}}
 
You can further divide the remaining space by 6, but 6 does not fit into 9, so you will still have 3 remaining
 {{< rawhtml >}}
<div class="center">
<img src="/images/tiles/6.png" style="width:400px;">
</div>
{{< /rawhtml >}}
Finally, if divide the last space by 3, since 3 fits perfectly into 6 you can finally cover the remaining space
{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/3.png" style="width:400px;">
</div>
{{< /rawhtml >}}
Now that you know that 3 is the largest common factor you can tile the entire floor.
// add file
Let’s summarize how we found the highest common factor¬¬ of a and b
                                
Play around with the exercise below to find more HCF


{{< rawhtml >}}
<div class="center">
<iframe 
        src="https://editor.p5js.org/lisa-pinto/full/7Ge_aRVU_"
        style="border-style: none;width: 800px; height: 550px"
         >
</iframe>
</div">
{{< /rawhtml >}}

{{< rawhtml >}}
<div class="center">
<img src="/images/formula.png" style="width:150px;box-shadow:none"><br>
So in the above example, it went like: <br>
<img src="/images/summary.png" style="width:150px;box-shadow:none">
</div>
{{< /rawhtml >}}

Summary
• Every number, when divided by another number will have a quotient and a remainder.
• If you keep on breaking the remainder down, you will eventually get the smallest factor pf the two numbers.