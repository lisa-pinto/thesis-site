---
author: Lisa
description: Pi with the Vitruvian Man
date: "2020-03-05"
image: tiles.webp
tags:
- emoji
title: Common Factors and pretty tiles
math: true
---

## Introduction

$$ 
sin^2(x)+cos^2(x)=1
$$

If you take a rectangular space, only a certain number of full-sized tiles will be able to fit into it. 
For simplicity, let us use square tiles
e.g. if you have a size of 25 and 30, you can use tiles of size 5, because 25 is equal to 5 full tiles and 30 is equal to 6 full tiles.

The Largest tiles that fit is called the Highest Common Factor


Euclid Developed a nifty trick that allows us to find out the largest tile that can fit an area.

{{< rawhtml >}}
<div class="center">
<img src="/images/euclid.jpg" style="width:400px;">
</div>
{{< rawhtml >}}

{{< rawhtml >}}
<div class="center">
<iframe 
        src="https://editor.p5js.org/lisa-pinto/full/W5iBROolh"
        style="border-style: none;width: 800px; height: 450px"
         >
</iframe>
</div">
{{< /rawhtml >}}




<br> Let’s Take The numbers 42 and 30.  
Since 30 is the smaller side, it is the largest possible tile size that can be used. 

You can only use maximum one tile of size 30, and you will have 12 remaining  
Let’s try to break the remaining piece down.   

You can use a maximum of 2 tiles of size 12 and you will have six remaining  
You can use exactly 2 tiles of size 6, and it will finally fill the space up  
Now that you know that six is the largest common factor  you can tile the entire floor. 



Let’s summarize how we found the highest common factor



{{< rawhtml >}}
<div class="center">
<iframe 
        src="https://editor.p5js.org/lisa-pinto/full/7Ge_aRVU_"
        style="border-style: none;width: 800px; height: 550px"
         >
</iframe>
</div">
{{< /rawhtml >}}