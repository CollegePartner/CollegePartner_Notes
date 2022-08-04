# Basic Electrical 2nd Sem Notes
## Course syllabus :-
### ***Module- I: DC Circuits***
Definition of electric circuit, linear circuit, non-linear circuit, bilateral circuit, unilateral circuit, Dependent source, node, branch, active and passive elements, Kirchhoff’s laws, Source equivalence and conversion.
Network Theorems - Superposition Theorem, Thevenin’s Theorem, Norton Theorem, Maximum Power Transfer Theorem, Star-Delta Conversions.

## DC Circuits
Dc Network theorems.

**Ideal Circuit elements are of two kinds :-**
1. **Passive Elements (R,L, C)-**

    Resistance is the dissipative element. Capacitance and inductance Can
    Store and deliver energy without any loss of energy in the Process, but their energy handling Capacity is limited.

    Practical Passive elements would Possess all the three Properties but depending upon their design one of these Properties will predominate.
    E.g.- Resistors, inductors, thermistors, and capacitors.
2. **Active Elements (Sources)-**

    Ideal Sources can handle infinite Power and energy. But Practical sources
can handle finite Power but infinite energy.
E.g.- A battery, transformer, semiconductors devices.
Certain Properties of ideal circuit elements (R, L,C).
These elements are:-
- Linear
- Bilateral
- Time invariant
- Lumped.
--- 
**(**Bilateral and Unilateral)**

R, L, C ideal elements behaviour is independent either of the terminal (node) at which current is fed in or of the direction of voltage applied at the terminals.

- **Bilateral:-** If the terminal Connections of an element in a circuit are reversed, it would not make any difference to the circuit response. This is the bilateral property of R, L, C elements. Bilateral elements offer the same impedance irrespective of the magnitude or direction of flow of current.

    **E.g.-** A resistor, an inductance and a capacitor, all are bilateral elements.

- **Unilateral:-** If the magnitude of the current passing through an element is affected due to change in polarity of the applied voltage, the element is called a unilateral element.Unilateral elements offer varying impedances with variation in the magnitude or direction of flow of the current.

    **E.g.-** Diodes, transistors, etc. are unilateral elements. 
-------
**Non-Linear and Linear**

- ***Non-linear:-*** Linear behaviour of an element is an approximation (idealisation) of general non-linear behaviour in a limited range of variables (Voltage/Current).
In other words, an electric circuit in which Circuit Parameters (Resistance,inductance, Capacitance, wove form, frequency etc) is not constant,Called non-linear Circuit.
**E.g.-**
    1. Diode
    2. Transistor
    3. Transformer
    4. Inductor


- ***Linear:-*** Linear circuit is an electrical circuit in which circuit parameters (Resistance, inductance, capacitance, wave form, frequency etc) are Constant. (A circuit Whose Parameters does not change with respect to current and Voltage is Called linear circuit).

    **E.g.-** Resistance, inductor, capacitor.
---
**Electric Circuits and Network Theorems:-**

There are certain theorems, which when applied to the solutions of electric networks, either simplify the network itself or render their analytical solution very easy. These theorems can also be applied to an a.c. system, with the only difference that impedances replace the ohmic resistance of
d.c. system. 

Different electric circuits (according to their properties) are defined below:

1. **Circuit.** A circuit is a closed conducting path through which an electric current either flows or is intended to flow.
2. **Parameters.** The various elements of an electric circuit are called its parameters like resistance, inductance and capacitance. These parameters may be lumped or distributed.
3. **Linear Circuit.** A linear circuit is one whose parameters are constant i.e. they do not with voltage or current.
4. **Non-linear Circuit.** It is that circuit whose parameters change with voltage or current.
5. **Bilateral Circuit.** A bilateral circuit is one whose properties or characteristics are the same in either direction. The usual transmission line is bilateral, because it can be made to per-form its function equally well in either direction.
6. **Unilateral Circuit.** It is that circuit whose properties or characteristics change with the direction of its operation. A diode rectifier is a unilateral circuit, because it cannot perform rectification in both directions.
7. **Electric Network.** A combination of various electric elements, connected in any manner whatsoever, is called an electric network.
8. **Passive Network** is one which contains no source of e.m.f. in it.
9. **Active Network** is one which contains one or more than one source of e.m.f.
10. **Node** is a junction in a circuit where two or more circuit elements are connected together.
11. **Branch** is that part of a network which lies between two junctions.
12. **Loop.** It is a close path in a circuit in which no element or node is encountered more than once.
13. **Mesh.** It is a loop that contains no other loop within it. 

---
## Kirchhoff's law

1. Kirchhoff's Point law or Current law (KCL)
In any electrical network, the algebraic Sum of the currents meeting at a Point (on junction) is Zero.

    The total current leaving a junction is equal to the total current entering that junction.

    Assuming the incoming currents to be Positive and the outgoing currents negative,

We have,

$$I_{1}+(-I_{2})+(-I_{3})+(+I_{4})+(-I_{5})=0$$
$$I_{1} + I_{4}- I_{2}- I_{3}-I_{5}= 0$$
$$or,I_{1} + I_{4} = I_{2}+ I_{3}+ I_{5}$$
$∴ incoming currents = outgoing currents.$

For, node A

    I1+(-I1)+(-I2)+(-I3)+(-I4)+(-I5)= 0.
    Or,I = I1 + I2 + I3 + I4 + I5.

We can express the above conclusion thus: ∑I = 0..at a junction

2. **Kirchhoff's Mesh law or Voltage law (KVL).**

    The algebraic sum of the Products of currents and resistances in each
    of the Conductors in any closed path (or mesh) in a network plus the algebraic sum of the e.m.f.s in that path is Zero.

        ∑IR + ∑emfs = 0.                             ____ round a mesh.
---
***Solving equations with two unknown Variables.***

 Let,

ax + by = c\
dx + ey = f

Here, the two unknown are x and y, a, b, d and e one coefficients of
these unknown whereas C and f are Constants.
### **#Steps**
1. write the matrix form as Δ =                                     


2. for finding the determinant fort, replace the coefficient of x in the original matrix by the Constants so that we get determinant Δ1 given by

3. By applying cramer's rule to get the value of x and y
---
### **Solving equations with three unknowns:-**
let the three equation be as :-
	    
        ax +by+ cz= d
	    ex + fy + yz=h
	    Jx + ky+ lz=m
 
---
### ***Independent and dependent Source-***
**Independent**  
Those voltages on current which does not depend on any other quantity in the Circuit, are Called independent Sources.\
**Dependent.**
A dependent Voltage or current source is one which depends on some other quantity in the Circuit, which may be either a voltage on a current. Such a source denoted by  ♢ so as not to confuse with an independent source
