---
layout: post
title: "How Big is a Circle?"
date: 2016-07-07
---

"Is everyone done? Good! Now draw a circle under the triangle in part 2, and count how many squares it fills up."

I looked at the graph paper in front of me, with a ruler in one hand and a pencil in another. Drawing the square was easy: tracing along the grid lines, 5 grids each, and it fills 25 squares perfectly. The triangle wasn't so bad either as long as I had a ruler. But now I'm supposed to draw a circle like this and count the grids:

![Grid Sheet](/images/circle/gridsheet.png)

Someone told me before that to draw a good circle you need a compass, but the teacher wouldn't let us use them in class because nobody likes those sharp ends, especially in the hands of kids. So if your drawing skills are anything like mine, it would probably come out as something like this:

![Bad Circle](/images/circle/badcircle.png)

I looked around at the other kids and their circles don't look much better. With one corner looking like a squished oval and another almost like a square, how are we supposed to count how many grids the circle covers? If we can barely even *draw* a circle, how can *anyone* figure out how big it is? 

------------------------------------------------------------------------------------------------------------------------------------

Not surprisingly, I wasn't the only one scratching my head about how big a circle is. Even the Ancient Greeks, who were masters of drawing perfect shapes, had a great deal of trouble figuring out a circle's area. To see why, let's take a step back and see how we have derived the area of other figures. 

First: the square. We can see that a square with a side length of n units covers n^2 square units of area. For example, a 5 by 5 square covers 25 square units of area. A rectangle is similar: a 6 by 3 rectangle covers 18 square units of area. In general, any rectangle of length m and width n covers m*n square units of area.

![rectangle](/images/circle/rectangle.png)

The picture gets somewhat more interesting when you have slanted sides, for example a triangle or a parallelogram. Let's focus on the parallelogram first. Calling one side the "base" (b) and the distance between the base and its opposite side the "height", we can reconstruct the parallelogram as a rectangle, with the original base and height as the new length and width, as follows:

![parallelogram](/images/circle/parallelogram.png)

Hence the area of a parallelogram is A=bh. From there on, we can show that a triangle can always be represented as half of some parallelogram, as follows:

![triangle](/images/circle/triangle.png)

Hence the area of any triangle is A=bh/2, where base and height are labelled in the diagram. Once we found the area of a triangle, it's game over for all polygons, since every polygon can be broken up into triangular pieces. Hence this is an incredibly powerful result.

![polygon](/images/circle/polygon.png)

In summary, the main method we used so far to measure complicated shapes is to break them up into smaller, simpler pieces. Once we can deconstruct or rearrange a complicated shape into pieces that we know how to calculate, we can solve the original area. However, this approach falls flat when we try to use it on the circle.

The big problem is that the perimeter of a circle is not a straight line, and all of the simple pieces we figured out so far have straight boundaries. There is also no obvious way of breaking apart a circle and rearranging them into one of the nicer shapes we figured out before. However, this deconstruction approach can still give us some intuitive insight on the size of a circle.

![badfit](/images/circle/badfit.png)

<h2>The Slicing Argument</h2> 

Let's say you are having a pizza party with seven of your friends. You cut the pizza into 8 equal pieces. But instead of distributing to your friends, you get the idea of rearranging these pieces to different shapes first. So you "flip" every other piece such that the first piece's tip is adjacent to the second piece's crust. Then you push the reorganized pieces together into a new shape, and realize that it kind of looks like a "wavy" parallelogram. If only the crusts were straight lines, it would be a parallelogram!

![8pizza](/images/circle/8pizza.png)

So then you cut the pizza into 16 pieces instead, and rearrange them into a wavy parallelogram using the same method. This time, you notices that while the two long opposing sides are still the wavy crusts, they are much straighter than the 8-piece version. If you cut the pizza into 32 pieces, the long sides (crusts) would look straighter still. In summary, the more slices you make, the straighter the two crust sides will become. 

[!16pizzacomp](/images/circle/16pizzacomp.png)

At each stage, we can approximate the area of the rearranged pizza ("wavy parallelogram") using a parallelogram defined by replacing the wavy crust sides with a pair of straight lines joining the same sets of endpoints, as shown in the above figure. Since the more slices we make, the straighter the two wavy crust sides will become, the straight line approximation will become closer and closer to the real wavy figure. Hence if we make many. many slices such that the resulting wavy parallelogram is almost a straight parallelogram, then the area of the wavy parallelogram (and thus the circle) is approximately the same as the area of the straight approximation. If we make infinitely many slices, there would be no difference between the resulting wavy parallelogram and its straight approximation.

Another thing to notice is that the more slices we make, the more *rectangular* the wavy parallelograms become. 
