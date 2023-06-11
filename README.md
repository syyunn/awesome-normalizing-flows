# awesome-normalizing-flows
Journey of studying and implementing normalizing flows

# What is Normalizing Flows?
A (finite) normalizing flow (NF), or flow, is an invertible function $f_\theta: \mathcal{X} \rightarrow \mathcal{Y}$ used to express a transformation between random variables. Since $f$ is invertible, the change of variables formula can be used to translate between densities $p_Y(\mathbf{y})$ and $p_X(\mathbf{x})$ :
$$
p_Y(\mathbf{y})=\left|\frac{\partial f(\mathbf{x})}{\partial \mathbf{x}}\right|^{-1} p_X(\mathbf{x})
$$

The -1 exponent in $\left|\frac{\partial f(\mathbf{x})}{\partial \mathbf{x}}\right|^{-1}$ indicates that we are taking the reciprocal (or inverse) of the absolute value of the Jacobian determinant.
Intuitively, the Jacobian determinant measures how much the function $f$ "stretches" or "shrinks" volumes in the input space. When transforming from one space to another, if the function $f$ stretches the space, then the local density should decrease, and if it shrinks the space, the local density should increase.

# Autoregressive Flows (Papamakarios, 2017)
It is advantageous to choose T to have an autoregressive structure such that Jacobian of $T:X \rightarrow Z$, $J_T(X)$ is a lower-triangular matrix and det $J_T (X)$ is just the product of the diagonal elements.


# Neural Autoregressive Flows (Huang, 2018)

