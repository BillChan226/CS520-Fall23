## Lecture 3

##### Convergence

The sequence below somehow does not converge. 
$$
X_k =
\left\{
\begin{aligned}
 \cos (\frac{2\pi k}{10} - 2^{-k}) \\
 \sin (\frac{2\pi k}{10} - 2^{-k})
\end{aligned}
\right.
$$
A sequence has a **limit point** or **accumulation point** when there is a subsequence that converges to $x^*$. 

If ${x_k}$ is the sequence;

then if $y_j = x_{k_j}$ (e.g. $y_j = x_{10j+1})$ is a new sequence and if $y_j \to y^*$ then $y^*$ is a limit point.

```julia
function seqvals(n)
  X = zeros(n, 2)
  for k=1:n
    X[k,1] = cos(2*pi*k/10 - 2.0^(-k))
    X[k,2] = sin(2*pi*k/10 - 2.0^(-k))
  end
  return X
end
```





