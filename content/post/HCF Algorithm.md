---
author: Lisa
description: Common Factors and pretty tiles
date: "2022-04-24"
image: tiles.webp
tags:
- emoji
title: Common Factors and Pretty tiles
math: true
---
#### Traditional Tile inlay
Various locations.
&nbsp;

&nbsp;


## Introduction

Many cultures in history have had their own traditional tiling arts. 

{{< rawhtml >}}
<div style="display: flex; width:100%;padding-left:10%;align-items: center; ">
<div style="padding:5%;justify-content: center;">
<img src="/images/azulejo.jpg" style="width:200px;"> 
<br> The Portuguese have traditional blue-and-white tiles called azulejo.
</div>
<div style="padding:5%;justify-content: center;">
<img src="/images/persian.jpg" style="width:200px;">
<br>Persian tiles are notable for their intricate geometry.
</div>
<div style="padding:5%;justify-content: center;">
<img src="/images/pietra.jpg" style="width:200px;">
<br>the Italians pioneered Pietra dura but was adopted by the mughals. 
</div>
</div>   
{{< /rawhtml >}}        

They all have one thing in common: They are based on patterns of smaller components fitting into a bigger space
&nbsp;

&nbsp;

## Finding Space for tiles

If you take a rectangular space, only a certain number of full-sized tiles will be able to fit into it. 

Let’s take Two variables, a and b  
(a has to be greater or equal to b)  

Let's make a = 39 and b = 15  
15 fits maximum two times into 39 (15 x 2 = 30), and you still have 9 left over  
 
{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/15_3.png" style="width:400px;">
</div>
{{< /rawhtml >}}

Now you have the equation $\longrightarrow$ 39 = 15(2) + 9
 
This is called Euclid’s Division Lemma, which states that:  
”For every two numbers a and b, there will be a number q (that is the maximum number of times that b fits into a), and r (a little bit left over), so that
a = b(q) + r
if b fits perfectly into a, then r will be 0."


To understand more, play around with the exercise below

{{< rawhtml >}}
<div class="center">
<div
style="
    width: 100%;
    height: 3.5rem;
    z-index:2;
    background: var(--bg);
    color: var(--bg);
    position: relative;"
></div>
<div style="margin-top:-3.5rem;z-index:1;position: relative;">
<iframe 
        src="https://editor.p5js.org/lisa-pinto/full/W5iBROolh"
        style="border-style: none;width: 800px; height: 450px"
         >
</iframe>
</div>
</div>
{{< /rawhtml >}}
&nbsp;

&nbsp;

## Finding tiles that fit

So far, we’ve been able to see how , many times a tile of size b fits into a. But can we find a number that fits into both b an a?

Once again Euclid Developed a nifty trick to solve the problem.
{{< rawhtml >}}
<div class="center">
<img src="/images/euclidbubble.png" style="width:500px;box-shadow:none">
</div>
{{< /rawhtml >}}

Let's See how Euclid's Division Algorithm works to fill up the space.

Let’s Take The numbers 39 and 15 again

The largest possible tile is 15,  
We know that 39 = 15(2) + 9, so you will have 9 remaining.

{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/15_3.png" style="width:400px;">
</div>
{{< /rawhtml >}}

Let’s try to break that remaining piece down.   
15 = 9(1) + 6, so you will still have 6 remaining
{{< rawhtml >}} 
 <div class="center">
<img src="/images/tiles/9_3.png" style="width:400px;">
</div> 
{{< /rawhtml >}}
 
9 = 6(1) + 3, so you will still have 3 remaining.

 {{< rawhtml >}}
<div class="center">
<img src="/images/tiles/6_3.png" style="width:400px;">
</div>
{{< /rawhtml >}}

<br>Finally, if divide the last space by 3,  
6 = 3(2) + 0,  
There is nothing left so you can fill the remaining space. 

{{< rawhtml >}}
<div class="center">
<img src="/images/tiles/3_3.png" style="width:400px;">
</div>
{{< /rawhtml >}}

<br>Through this factor, we have concluded that 3 is a factor of both 15 and 39, so you can use it to till the whole floor.  

{{< rawhtml >}}
<div class="center">
<img src="/images/allhcf.png" style="width:400px;">
</div>
{{< /rawhtml >}}

<br>Let’s summarize how we found the highest common factor of a and b  

 {{< rawhtml >}}
<div class="center">
<img src="/images/nsummary.png" style="width:150px;box-shadow:none"><br>
So the process can be simplified as: <br>
<img src="/images/nformula.png" style="width:150px;box-shadow:none">
<br> until you reach 0
</div>
{{< /rawhtml >}} 
&nbsp;

&nbsp;

Play Around below to see more break-downs

{{< rawhtml >}}
<div class="center">
<div
style="
    width: 100%;
    height: 3.5rem;
    z-index:2;
    background: var(--bg);
    color: var(--bg);
    position: relative;"
></div>
<div style="margin-top:-3.5rem;z-index:1;position: relative;">
<iframe 
        src="https://editor.p5js.org/lisa-pinto/full/7Ge_aRVU_"
        style="border-style: none;width: 800px; height: 550px"
         >
</iframe>
</div>
</div>
{{< /rawhtml >}}


#### Summary  
• Every number, when divided by another number will have a quotient and a remainder.  
• The gives the equation a = b(q) + r, for any a and b  
• If you keep on breaking the remainder down, you will eventually get the highest factor of the two numbers.  