# advanced-machine-learning
Theoretical analysis of Machine Learning algorithms. Assignments from AI master at University of Bucharest.

> ::notebook_with_decorative_cover:: *LaTeX is not supported in GitHub's markdown files: For better formatting, jump to my PDF solutions*.


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

**Exercise 6**. Let X be an instance space and consider H ⊆ {0,1}^X a hypothesis space with finite VC dimension. For each 𝑥 ∈ X, we consider the function z_x : H →{0,1} such that z_x(h) = h(x) for each ℎ ∈ H. Let Z = {z_x : H→{0,1}, 𝑥 ∈ X}. Prove that VCdim(Z) < 2^{VCdim(H)+1}.


### Assignment 2

Check my solution is [here](AML__Assignment_2.pdf).

**Exercise 1**. Let X be an instance space. The learning algorithm A is better than the learning algorithm B with respect to some probability distribution, D, if we have: L_D(A(S)) ≤ L_D(B(S)) for all samples S ∈ (X × {0,1})^m. Prove that for every distribution D over X × {0,1} there exist a learning algorithm A_D that is better than any other algorithm with respect to D.

**Exercise 2**. Consider H to be the class of concentric circles centered in origin in the 2D plane. Consider the realizability assumption.
- show that the class H can be (𝜖, 𝛿) − PAC learned by giving the algorithm A and determining the sample complexity m_H(𝜖, 𝛿) such that the definition of PAC-learnability is satisfied.
- compute VCdim(H).

**Exercise 3**. Consider the concept class C formed by closed intervals [a,b] with a,b ∈ ℝ: C = {h_a,b : R→{0,1}, a ≤ b, h_a,b(𝑥) = 𝟏[a, b]\(𝑥)}.
Compute the shattering coefficient 𝜏_H(𝑚) of the growth function for m ≥ 0.

**Exercise 4**. Consider de concept class C 2 formed by union of two closed intervals, that is [𝑎, 𝑏] ∪ [𝑐, 𝑑], with a, b, c, d ∈ R (with a ≤ b ≤ c ≤ d). Give an efficient ERM algorithm for learning the concept class C₂ and compute its complexity for each of the following cases:
- realizable case.
- agnostic case.

**Exercise 5**. Consider H2DNF^d the class of 2-term disjunctive normal form formulae consisting of hypothesis of the form h: {0,1}^d → {0,1}, h(x) = A₁(x) ∨ A₂(x), where Aᵢ(x) is a Boolean conjunction of literals (in Hconj^d).
It is known that the class H2DNF^d is not efficient properly learnable but can be learned improperly considering the class H2CNF^d. Give a γ-weak-learner algorithm for learning the class H2DNF^d which is not a stronger PAC learning algorithm for H2DNF^d (like the one considering H2CNF^d). Prove that this algorithm is a γ-weak-learner algorithm for H2DNF^d.