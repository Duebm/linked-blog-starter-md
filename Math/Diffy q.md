[[ODE]]


[[Methods of Solving ODEs]]


[[Well posited]]


[[Graphical notation]]



## Exam 2

#### - Basic generalization of higher order ODEs (constant coeff)
Generalize the thang: v'' - 6v' +9v = 4e^3t
z^2 - 6z + 9 = (z-3)^2

Blueprint: y(t)=c1y1(t)+c2y2(t)

(z-3)^2 is a "repeated root"- so we add a "t" in front of c2

y(t)= c1 e^3t + c2 t e^3t
Take the derivative of this to get a second eq., then solve for c1 and c2 
y'(t)= 3 c1 e^3t + 3t c2 e^3t

### - non-homogenion

- Take the general version of the homogenous sde, then add the "partiular "solution for the right side of equ.
	- Undetermined coeff
		- Guesswork
		- Hard when the forcing is fucked (cos or sin or i)
	- Key identidy
	- Variation of paremetiers 
		- Varitation of parameters usable always 

- These three give just the pariticuar sol., you still need to solve for the homogenous sol.

####  - Wronskian hehe

Wr (y1,y2) (t) = det [y1(t) y2(t)
                y1'(t) y2'(t)]

- If Wr does not = 0, then it is a fundamental set of solutions 

#### - Variation of parameters

x^2 y'' - 6xy' + 10y = x^6 cos2x

Given homogenuous solutions x^2 and x^5

x^2 u1' + x^5 u2' = 0
- Set equal to forcing term
- Solve for u1' and u2' 
- Integrate to get u1 and u2



#### - key identdy method
- CONSTANT COEFF

y''-2y'+2y = 100 cos2t
z^2 - 2z +2 = 0
z= 1 plus or minus i

"chasteristic" =2i for this

D^2 -2D +2

(-2-4i) is from plugging in the characteristic into the D equation

L(e^2it) = (-2-4i)e^2it
L(-1/(2+4i) e^2it) = e^2it
L(Re()


### - undetermined coeff

w'' - 4w' +5w = e^2x
- Guess a solution based off of the forcing 
Guess: Ae^2x is a sol.

(4A - 8A + 5A)e^2x = e^2x

A = 1

ex) 

w'' - 4w = e^2x
 p^2 - 4 = 0 

c1 e^2x + c2 e^-2x

A x e^2x

(xe^2x) = (2x+1) e ^2x

#### - La place transforms 

y'' + 4y' - 21y = 0
y(0) = 2, y'(0) = 3

- Remove the higher order using the equations u had on quiz

- Do the laplace based off of formulas on formula sheet

- Do the laplace of the forcing
- Simplfiy
- Do the inverse laplace 
	- NEED TO KNOW PARTIAL FRACTIONS

### - piecewise forcing


