## Image Reconstruction by Splitting Deep Learning Regularization from Iterative Inversion

### Image Reconstruction problems
fast MRI
  - partial 2D Fourier transform
  
low dose CT
  - X-ray transform
  
### Idea
We do not intend to learn an end-to-end inversion mapping from the measurements to 
the reconstructed image as previous work.

data consistence is maintained through iteration for the reconstruction.


<script type="text/javascript" async src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML"> </script>
formula1: $$n==x$$

formula2: $$n!=x$$

formula3: (m==y)

formula4: [m!=y]

formula5: \(k==z\)

formula6: \[k!=z\]

$$ J(x) = \eta (\sum_{i=1}^m ||Ax_i - y_i||_2^2+\mu || Dx_i||_1)$$
