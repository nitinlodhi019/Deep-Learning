# 1. Feature Extraction

- Definition: Using a pre-trained model as a fixed feature extractor. You don’t change the weights of the pre-trained layers. You only train a new classifier on top.

- Key Idea: The pre-trained CNN already learned useful features (like edges, textures, shapes), so you just use them for your task.

- Typical Steps:

  1. Take a pre-trained CNN (e.g., ResNet, VGG).
  
  2. Remove the final classification layer.
  
  3. Freeze all convolutional layers (weights don’t update).
  
  4. Add a new output layer for your task.
  
  5. Train only the new output layer on your dataset.

- When to Use:

Small dataset.

Task is similar to original pre-trained task.

✅ Example: Use pre-trained VGG trained on ImageNet to classify flowers, just training the last dense layer.

2. Fine-Tuning

Definition: Starting with a pre-trained model but unfreezing some or all layers and training them on your dataset, so the model adapts its features to the new task.

Key Idea: You allow the network to slightly adjust the learned features to better fit your dataset.

Typical Steps:

Take a pre-trained CNN.

Freeze initial layers (optional) and unfreeze deeper layers.

Add a new output layer.

Train on your dataset with a smaller learning rate to avoid destroying pre-trained knowledge.

When to Use:

Moderate to large dataset.

Task is different from the original pre-trained task.

✅ Example: Fine-tune ResNet trained on ImageNet to classify medical X-ray images.

Key Differences
Aspect	Feature Extraction	Fine-Tuning
Layers Trained	Only new output layer	Some or all pre-trained layers + new layer
Weights Update	Frozen (no updates)	Partially or fully updated
Dataset Size	Small	Moderate to large
Task Similarity	Similar to pre-trained task	Can be different from pre-trained task
Flexibility	Less flexible	More flexible
Risk of Overfitting	Low	Higher
In short:

Feature Extraction: Use pre-trained CNN as-is; just train the new classifier.

Fine-Tuning: Adjust pre-trained weights slightly to adapt to your dataset.
