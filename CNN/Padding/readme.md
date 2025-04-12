![image](https://github.com/user-attachments/assets/2b927f7a-a76f-475d-8ef0-5e84ba9fe2da)


# **🧱 What is Padding?**

Padding means adding extra pixels around the border of an image — usually filled with zeros (but sometimes other values). This is done before applying convolution.

## **📸 Why Do We Need Padding?**

Let’s say you have:

* A 5x5 grayscale image.

* A 3x3 filter (kernel).

When you convolve without padding:

* The output image becomes (5−3+1) × (5−3+1) = 3×3

* You lose pixels on the borders because the filter can’t “slide” beyond the edges.

**Padding helps you:**

1. Preserve original image size after filtering.

2. Let filters see edge pixels.

3. Avoid shrinking the image with each convolution.

## **🧮 Types of Padding**

**1. Zero Padding (Most common)**

* Add zeros around the border.

**2. Same Padding**

* Output size = Input size

* Padding depends on kernel size:

* For 3x3 kernel → pad = 1 (on each side)

* For 5x5 kernel → pad = 2

**3. Valid Padding**

* No padding applied.

* Output is smaller than input.

* Just valid positions where the filter fits completely.

## **✅ Quick Rule of Thumb for Padding Size**

For a square filter of size k × k:

pad = (k - 1) // 2

E.g., 3×3 filter → pad = 1
