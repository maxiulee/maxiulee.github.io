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

Hence the area of any triangle is A=bh/2, where base and height are labelled in the diagram. This is a very powerful result: since *any* shape enclosed by straight lines can be broken up into triangles, this gives us a fool-proof (although tedious) method of finding the area of any such shape.

![polygon](/images/circle/polygon.png)

In summary, the main method we used so far to measure complicated shapes is to break them up into smaller, simpler pieces. 

