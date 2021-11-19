# advanced-machine-learning
Theoretical analysis of Machine Learning algorithms. Assignments from AI master at University of Bucharest.

### Assignment 1

Check my solution is [here](AML__Assignment_1.pdf).

**Exercise 1**. Give an example of a finite hypothesis class H with VCdim(H) = 2021.
Justify your choice.

**Exercise 2**. Consider H balls to be the set of all balls in R²: H balls = {B(x,r), x ∈ ℝ² , r ≥ 0 }, where B(x,r) = {y ∈ ℝ 2 | || y – x ||₂ ≤ r}. As mentioned in the lecture, we can also view H_balls as the set of indicator functions of the balls B(x,r) in the plane.
Can you give an example of a set A in R² of size 4 that is shattered by H balls ? Give such an example or justify why you cannot find a set A of size 4 shattered by H_balls .


**Exercise 3**. Let X = R² and consider Hα the set of concepts defined by the area inside a right triangle ABC with the two catheti AB and AC parallel to the axes (Ox and Oy) and with AB / AC = α (fixed constant > 0). Consider the realizability assumption. Show that the class H_α can be (𝜖, 𝛿) − PAC learned by giving an algorithm *A* and determining an upper bound on the sample complexity m_H(𝜖, 𝛿) such that the definition of PAC-learnability is satisfied.


**Exercise 4**. Consider H to be the class of all centered in origin sphere classifiers in the
3D space. A centered in origin sphere classifier in the 3D space is a classifier h_r that assigns the value 1 to a point if and only if it is inside the sphere with radius r > 0 and center given by the origin O(0,0,0). Consider the realizability assumption.

- show that the class H can be (𝜖, 𝛿) − PAC learned by giving an algorithm A and determining an upper bound on the sample complexity m_H(𝜖, 𝛿) such that the definition of PAC-learnability is satisfied.
- compute VCdim(H).


**Exercise 5**. Let H = {ℎ_𝜃 : ℝ → {0, 1} , ℎ_𝜃(𝑥)  = 𝟏[𝜃, 𝜃+1]∪[𝜃+2, ∞)(𝑥), 𝜃 ∈ ℝ}. Compute VCdim(H).

**Exercise 6**. Let X be an instance space and consider H ⊆ {0,1}^X a hypothesis space with finite VC dimension. For each 𝑥 ∈ X, we consider the function z_x : H →{0,1} such that z_x(h) = h(x) for each ℎ ∈ H. Let Z = {z_x : H→{0,1}, 𝑥 ∈ X}. Prove that VCdim(Z) < 2^{VCdim(H)+1} .