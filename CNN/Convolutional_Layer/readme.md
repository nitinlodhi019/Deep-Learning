[https://anhreynolds.com/img/cnn.png](https://www.google.com/url?sa=i&url=https%3A%2F%2Fanhreynolds.com%2Fblogs%2Fcnn.html&psig=AOvVaw3gokIBvvptrgKEts6tg5f0&ust=1744524759973000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCIiayKnr0YwDFQAAAAAdAAAAABAL)



**🔍 What is a Convolutional Layer?**

A Convolutional Layer is the core building block of a CNN. It’s responsible for extracting features from the input image—things like edges, textures, shapes, and more complex patterns as you go deeper.

**⚙️ How it Works:**

Imagine sliding a small window (called a filter or kernel) over the image. This filter looks at a portion of the image and computes a value. Here's the breakdown:

1. Filter/Kernel: A small matrix (e.g., 3x3 or 5x5) with learnable weights.

2. Stride: How many pixels the filter moves at a time.

3. Padding: Adds extra pixels around the border so that the output size can be controlled.

**Convolution Operation:**

The filter "slides" over the image.

At each position, it multiplies its weights with the corresponding image values (element-wise), sums them up, and stores the result in the output feature map.

This helps detect patterns like vertical or horizontal edges, corners, etc.

**🧠 Why It's Powerful:**

Instead of learning from the entire image all at once (like a fully connected layer), it focuses on local patterns.

It drastically reduces the number of parameters.

Multiple filters can be applied in one layer to detect different features.
