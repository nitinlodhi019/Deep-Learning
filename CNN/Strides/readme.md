# **🚶‍♂️ What is Stride?**

A stride defines how much the filter/kernel moves across the input image or feature map during the convolution operation.

* Stride = 1: the filter moves one pixel at a time (default).

* Stride = 2: the filter jumps two pixels at a time, reducing the output size more quickly.

* Larger strides mean fewer output values, i.e., downsampling.


# **🔥 When to Use Higher Strides?**

* When you want faster computation.

* When you want to reduce feature map size without using pooling.

* In architectures like MobileNet, higher strides help keep the model lightweight.

# **🎯 Why Do We Use Strides in CNNs?**

**1. 🧹 Reduce the Output Size**
   
A larger stride reduces the spatial dimensions of the output (height and width).

This helps in downsampling the feature maps without needing a separate pooling layer.

Reducing size helps in managing computational cost and memory usage.

**2. ⚡ Improve Computational Efficiency**

With larger strides, the convolution operation is performed fewer times, so the model trains faster and requires less processing power.

**3. 🕵️‍♂️ Extract Global Features**

* *Small strides = local features (fine details)*

* *Large strides = more abstract, global features by skipping fine details.*


They keep the model lighter and faster without adding extra layers.
