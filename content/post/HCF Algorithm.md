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

Many cultures in history have had their own traditional tiling arts  

{{< rawhtml >}}
<div style="display: flex; width:100%;padding-left:10%;align-items: center; ">
<div style="padding:5%;justify-content: center;">
<img src="/images/azulejo.jpg" style="width:200px;"> 
<br> The Portuguese have traditional blue-and-white tiles called azulejo.
</div>
<div style="padding:5%;justify-content: center;">
<img src="/images/persian.jpg" style="width:200px;">
<br>Persian tiles are notable for their intricate geometry
</div>
<div style="padding:5%;justify-content: center;">
<img src="/images/pietra.jpg" style="width:200px;">
<br>Pietra dura was started by the italians but was widely used by the mughals. 
</div>
</div>   
{{< /rawhtml >}}        

They all have one thing in common: They are based on Patterns of smaller components fitting into a bigger space

## Finding Space for tiles

If you take a rectangular space, only a certain number of full-sized tiles will be able to fit into it. 

Let’s take Two variables, A and B  
(A has to be greater or equal to B)  

Let's make A = 39 and B = 15  
15 fits two times into 39, and you still have 9 left over  
 
{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/15.png" style="width:400px;">
</div>
{{< /rawhtml >}}

Now you have the equation $\longrightarrow$ 39 = 15(2) + 9
 
This is called Euclid’s Division Lemma, which states that:
”For every two numbers a and b, there will be a number q (that is the number of times that b fits into a), and r (a little bit left over), so that
a = b(q) + r
if b fits perfectly into a, then r will be 0.


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

## Finding tiles that fit

So far, we’ve been able to see how , many times a tile of size b fits into a. But can we find a number that fits into both b an a?

Once again Euclid Developed a nifty trick to solve the problem.
{{< rawhtml >}}
<div class="center">
<img src="/images/euclidbubble.png" style="width:500px;box-shadow:none">
</div>
{{< /rawhtml >}}

Let’s Take The numbers 39 and 15 again
Since 15 is the smaller side, it is the largest possible tile size that can be used. 
We already know that the biggest possible tile is 15, and you will have 9 remaining.  

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

{{< rawhtml >}}
<div class="center">
<img src="/images/allhcf.png" style="width:400px;">
</div>
{{< /rawhtml >}}
Let’s summarize how we found the highest common factor of a and b

{{< rawhtml >}}
<div class="center">
<img src="/images/summary.png" style="width:150px;box-shadow:none"><br>
So the process can be simplified as: <br>
<img src="/images/formula.png" style="width:150px;box-shadow:none">
<br> until you reach 0
</div>
{{< /rawhtml >}}
                                
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


Summary  
• Every number, when divided by another number will have a quotient and a remainder.  
• If you keep on breaking the remainder down, you will eventually get the smallest factor pf the two numbers.  