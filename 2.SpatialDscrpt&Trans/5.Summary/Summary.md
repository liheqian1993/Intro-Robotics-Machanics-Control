&emsp;
# Summary

We have introduced concepts first for the case of translation only, then for the case of rotation only, and finally for the general case of rotation about a point and translation of that point. Having understood the general case of rotation and
translation, we will not need to explicitly consider the two simpler cases since they are contained within the general framework.

As a general tool to represent frames, we have introduced the homogeneous transform, a $4 \times 4$ matrix containing orientation and position information.

We have introduced three interpretations of this homogeneous transform:
1. It is a description of a frame. ${ }_B^A T$ describes the frame $\{B\}$ relative to the frame $\{A\}$. Specifically, the columns of ${ }_B^A R$ are unit vectors defining the directions of the principal axes of $\{B\}$, and ${ }^A P_{B\ O R G}$ locates the position of the origin of $\{B\}$.

2. It is a transform mapping. ${ }_B^A T$ maps ${ }^B P \rightarrow{ }^A P$.
3. It is a transform operator. $T$ operates on ${ }^A P_1$ to create ${ }^A P_2$.


From this point on, the terms frame and transform will both be used to refer to a position vector plus an orientation. Frame is the term favored in speaking of a description, and transform is used most frequently when function as a mapping or operator is implied. 

Note that transformations are generalizations of (and subsume) translations and rotations; we will often use the term transform when speaking of a pure rotation (or translation).