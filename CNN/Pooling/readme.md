# **🧠 What is Pooling?**

Pooling is a downsampling operation used in CNNs to reduce the spatial dimensions (width and height) of the feature maps while retaining the most important features.

It is usually applied after a convolutional layer.

## **🎯 Why Do We Use Pooling?**

**Purpose**                                         **Benefit**

* 🧹 Reduces spatial dimensions	                    Makes computation faster and reduces memory usage
  
* 🔍 Retains essential features	                      Keeps important patterns while discarding unimportant details

* 🛡️ Reduces overfitting	                            Fewer parameters = less chance of memorizing training data

* 🔄 Provides translation invariance	                Small shifts in the image won't change the output much

## **📦 Types of Pooling**

**1. Max Pooling**

Picks the maximum value in a given window (e.g., 2x2)

Most common in practice
