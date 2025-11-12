# Visualizing Filters of a Convolutional Neural Network (CNN)

## Overview
This project demonstrates how convolutional neural networks (CNNs) learn and detect visual patterns by visualizing their internal filters.  
Using **TensorFlow** and the **VGG16** model, each layer’s learned features—ranging from simple edges to complex textures—were visualized to better understand how CNNs interpret and represent image data.

The goal was to create a clear, interpretable view of what each convolutional layer focuses on during image processing.


## Project Display

Model: vgg16 

<img width="565" height="598" alt="image" src="https://github.com/user-attachments/assets/6c07a909-d354-42d3-8258-02dab93a591c" />

Layer Outputs

<img width="555" height="157" alt="image" src="https://github.com/user-attachments/assets/a5e7aef3-c8dd-4685-894c-4f49e5bf3071" />

Image Visualization

<img width="324" height="342" alt="image" src="https://github.com/user-attachments/assets/3caa7965-b0ac-4f4a-b722-8a28a069d23e" />

Some Final Outputs
You can find the rest of the results in the accompanying .ipynb file in this repository.

<img width="330" height="673" alt="image" src="https://github.com/user-attachments/assets/4dcb9df0-56fa-478e-b61c-dc0edd7213fa" />
<img width="319" height="689" alt="image" src="https://github.com/user-attachments/assets/1f55811d-c9fb-4a86-be4f-8f36d7ab388c" />

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


