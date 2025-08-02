## Analyzed 3 different approaches to implementing convolutions, treating pytorch's implementation as a reference implementation.
In first approach, followed a naive nested for loop based implementation
For second approach, used matrix multiplication and reduced the degree of for-loop nesting to 2
For third approach, rearranged elements of input image inorder to completely perform convolution as a matrix multiplication
## Comparison of runtimes for the 3 approaches:

| Approach | Convolution time |
| --- | --- |
| Pytorch's implementation | 3.96 ms |
| 7 nested for-loops | 11.9s |
| Matmul approach with 2 nested for-loops | 16 ms| 
| im2col based matmul approach | 8.31 ms |
