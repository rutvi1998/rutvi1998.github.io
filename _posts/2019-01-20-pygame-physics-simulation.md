---
layout: post
title:  "Pygame Physics Simulations"
date:   2019-01-20
excerpt: "Simple and interactive Pygame Physics Simulations that demonstrate some concepts from standard XI Physics."
project: true
tag:
- pygame 
- physics
- simulations
comments: false
---

This project comprises of three, simple and interactive, physical simulations built using Python and Pygame. 
These simulations have been captioned Falling Balls, Discs on Table and Coalescence of Particles, 
respectively. One can understand the concepts used in the implementation of these three simulations by 
refering to a standard XI Physics textbook.

Like I said, the technology used in this project is limited to Python and Pygame. Some formulas that play 
an important role in the implementation of this project include the following :
	
**1) To determine velocity of balls after collision...**  

  v1 = (m1 – m2 / m1 + m2) * u1 + (2 * m2 / m1 + m2) * u2   
 	
  v2 = (m2 – m1 / m1 + m2) * u2 + (2 * m1 / m1 + m2) * u1   
 
(coefficient of elasticity (e) = 1)
 
The above formula has been derived from the equations given below :
  m1 * u1 + m2 * u2  =  m1 * v1 + m2 * v2  (conservation of momentum)
	
  1/2 * m1 * u1 * u1 + 1/2 * m2 * u2 * u2 =  1/2 * m1 * v1 * v1 + 1/2 * m2 * v2 * v2 (conservation of 
  kinetic energy)

**2) To estimate force of attraction between two particles...**

  F = G * m1  * m2 / r * r 

**3) To find position and velocity of the new particle after coalescence of two particles...**

  x = (m1 * x1  + m2 * x2) / m1 + m2 

  y = (m1 * y1  + m2 * y2) / m1 + m2 

  v = (m1 * v1  + m2 * v2) / m1 + m2

If you wish to study this project more thoroughly, please check out the project here... 

{% highlight yaml %} 
    url: https://github.com/rutvi1998/Zense-Project 
{% endhighlight %}

Meanwhile, I have some screenshots that you can view to see how these simulations look!

**1) balls.py**

{% capture images %}
   https://user-images.githubusercontent.com/43961129/51442929-37864100-1d08-11e9-9020-f2fac2862ff7.png
{% endcapture %}
{% include gallery images=images cols=1 %}

**2) discs.py**

{% capture images %}
  https://user-images.githubusercontent.com/43961129/51442932-3bb25e80-1d08-11e9-908b-5e2ea9969d5b.png
{% endcapture %}
{% include gallery images=images cols=1 %}

**3) coalescence.py**

{% capture images %}
  https://user-images.githubusercontent.com/43961129/51442931-39500480-1d08-11e9-813b-56892f65b506.png 
{% endcapture %}
{% include gallery images=images cols=1 %}


### Thank you!
