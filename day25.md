Lesson 6: Feature Vector, CIFAR Classification Example, CNN Classification

Summary note: https://docs.google.com/document/d/1o0oHRQx_sxns6B6CZzrg7YC-g441V4VR1NIHTGlDy6Y/edit?usp=sharing

Code Google Colab:

https://github.com/vsay01/deep-learning-v2-pytorch/blob/lesson6/convolutional-neural-networks/cifar-cnn/cifar10_cnn_exercise.ipynb

Note:

- In the CIFAR10_CNN Notebook, I achieved overall test accuracy of 72 %

![result](https://docs.google.com/uc?id=11sO7IlyDmGiNCPAJWSouQ6OHWXfWbIZq)

- In that notebook exercise at the section visualize sample test results, there's an issue:

TypeError: can't convert CUDA tensor to numpy. Use Tensor.cpu() to copy the tensor to host memory first.

To resovlve this make sure to use cpu as 

```imshow(images.cpu()[idx])```
