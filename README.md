# Visualizing Filters of a Convolutional Neural Network (CNN)

## Overview
This project demonstrates how convolutional neural networks (CNNs) learn and detect visual patterns by visualizing their internal filters.  
Using **TensorFlow** and the **VGG16** model, each layer’s learned features—ranging from simple edges to complex textures—were visualized to better understand how CNNs interpret and represent image data.

The goal was to create a clear, interpretable view of what each convolutional layer focuses on during image processing.


## Project Display


Example placeholder:  
`![Filter Visualization Example](images/filter_visualization.png)`



## Methodology
1. **Model Setup:**  
   Used the pre-trained **VGG16** architecture (`include_top=False`) for feature extraction.

2. **Submodel Creation:**  
   Extracted specific convolutional layers (e.g., `block1_conv2`, `block2_conv1`) using TensorFlow’s Functional API for focused visualization.

3. **Image Generation:**  
   Initialized random input images and iteratively optimized them to maximize filter activations using gradient ascent.

4. **Visualization:**  
   Displayed activation patterns across layers to illustrate how features evolve from low-level edges to high-level textures.

5. **Evaluation:**  
   Compared loss improvements and visual differences across iterations (e.g., iteration 10 vs. 100) to observe the model’s learning progression.

## Results
- **Early layers** captured basic edge and color patterns.  
- **Deeper layers** revealed more abstract and textured structures.  
- Filter activations became more refined as optimization proceeded, confirming CNNs’ hierarchical feature extraction mechanism.


## Technologies and Tools
- **Frameworks:** TensorFlow 2.17.1, Keras  
- **Model:** Pre-trained VGG16 (without top layers)  
- **Programming Language:** Python  
- **Environment:** Google Colab  
- **Visualization Libraries:** Matplotlib, NumPy  


