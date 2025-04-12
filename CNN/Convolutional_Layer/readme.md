**For GrayScale Image**

![image](https://github.com/user-attachments/assets/5ad346e5-b8ce-4ece-a883-ce8efe72daea)

**For RGB Image**

![image](https://github.com/user-attachments/assets/55bffef9-2cfc-4a5f-92f5-28b1612dc959)

after applying filter on a RGB image channels depends on the number of filters use.

input image = 6 x 6(n1 x n2) 

filter = 3 x 3(m1 x m2)

output image = (n1-m1+1) x (n2-m2+1)

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
