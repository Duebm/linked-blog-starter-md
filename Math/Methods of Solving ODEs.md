There are many methods of solving [[ODE]]s, they are used in a patchwork similar to calc 3
 ***
 
**Integrating Factor (M)** - 
Used for solving first order ODEs 
1. Isolate the constant in the equation 
2. Multiply the ODE by M
	- (dy/dt) (M) + (M)(yt^2)
	- M= e^intyt2
	- In this example it is (yt^2) b/c that is the rest of the equation 
3. Use the inverse of the product rule

***

**Euler's Method

- Used when not separable 
- General form for Euler's exactness test: dy/dx + M(x,y)/ N(x,y) = 0
- If dy (M(x,y)) = dx (N(x,y)), then is exact 

**Steps: 

1. Some H exists such that 
	1. M(x,y)= dx (H(x,y))
	2. N(x,y)= dy (H(x,y))
2. Solve for H by integrating one of them
	1. ex: integral of M(x,y)= H(x,y) = e^x + 2x +H(y)
3. Plug into the other equation 
	1. dy * e^x + 2x + H(y)= N(x,y)
	2. 
