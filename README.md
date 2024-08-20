# Advanced Skin Cancer Detection using Enhanced U-Net with SE and CBAM

This project focuses on enhancing skin cancer detection by developing a cutting-edge model that integrates Squeeze-and-Excite (SE) blocks and Convolutional Block Attention Modules (CBAM) into a U-Net architecture. Our innovative approach significantly improves the precision of segmenting skin cancer lesions, particularly those with complex and irregular shapes.

## Key Contributions

### Architectural Development
We designed a novel U-Net model that integrates SE and CBAM, enhancing feature extraction and reducing noise for more accurate lesion detection. This architecture is particularly effective in identifying complex and irregularly shaped skin cancer lesions.

### Data Augmentation
To improve the model's ability to generalize across diverse skin types and conditions, we employed advanced data augmentation techniques. These techniques include rotation, flipping, scaling, and contrast adjustments. These augmentations help to create a more diverse dataset, enabling the model to perform well in various real-world scenarios.

### Outstanding Results
Our model achieved superior performance on the ISIC dataset, demonstrating high scores in key metrics such as Dice Coefficient, Intersection over Union (IoU), and Binary Accuracy. These results indicate the model's robustness and accuracy in segmenting skin cancer lesions.

### Comparative Success
In comparison to existing methods, our model outperformed the industry standards by achieving a 12% performance boost. This marks a significant advancement in the early detection of melanoma, with the potential to improve clinical outcomes by enabling more accurate and earlier diagnosis.

## Project Architecture

The architecture of our model is based on the U-Net, enhanced by integrating Squeeze-and-Excite (SE) blocks and Convolutional Block Attention Modules (CBAM). Additionally, we incorporated a Multi-head Attention mechanism before the bottleneck layer. These enhancements allow the model to better focus on relevant features while reducing the impact of noise, leading to more precise segmentation results.

![Architecture](git-pics/architecture.png)

- **Trainable Parameters**: 8,634,593 (32.94 MB)

## Data Augmentation Techniques

To further enhance the model's performance, we applied various data augmentation techniques, including:

- **Rotation**: Random rotations to simulate different orientations of the skin lesions.
- **Flipping**: Horizontal and vertical flipping to increase data variability.
- **Scaling**: Random scaling to simulate different sizes of lesions.
- **Contrast Adjustments**: Altering the contrast to simulate different lighting conditions.

These augmentations helped to create a more diverse dataset, enabling the model to generalize better across different types of skin and conditions.

## Implementation Details

The model was implemented using Python, with TensorFlow and NumPy as the primary frameworks. The key components of the architecture include:

- **U-Net Backbone**: A well-known architecture for image segmentation tasks.
- **Convolutional Block Attention Modules (CBAM)**: Added to enhance the model's ability to focus on important features.
- **Squeeze-and-Excite (SE) Blocks**: Incorporated to improve the network's channel-wise feature recalibration.
- **Multi-head Attention**: Integrated before the bottleneck layer to further refine the features.

Through extensive trials and continuous hyper-parameter tuning, we were able to achieve a significant improvement over existing models.

## Performance Metrics

Our model's performance was rigorously evaluated on the ISIC dataset, resulting in impressive metrics:

- **Dice Coefficient**: A high score indicating the model's accuracy in overlapping regions between the predicted segmentation and the ground truth.
- **IoU (Intersection over Union)**: A measure of the overlap between the predicted segmentation and the actual lesion area.
- **Binary Accuracy**: Reflects the model's ability to correctly classify pixels as part of the lesion or not.

Below are the accuracy and loss graphs over 100 epochs, demonstrating the model's training process:

![Accuracy and Loss](git-pics/pic-1.png)
![Accuracy and Loss](git-pics/pic-2.png)
![Accuracy and Loss](git-pics/pic-3.png)
![Accuracy and Loss](git-pics/pic-4.png)
![Accuracy and Loss](git-pics/pic-5.png)

## Model Results

The effectiveness of our model is further illustrated by the following examples, which show how the model accurately segments skin cancer lesions:

![Example 1](git-pics/example-1.png)
![Example 2](git-pics/example-2.png)
![Example 3](git-pics/example-3.png)

## Conclusion

This research makes a significant academic contribution to the field of skin cancer detection. By improving the precision and early diagnosis capabilities of the model, it has the potential to positively impact clinical outcomes, enabling earlier and more accurate treatment of skin cancer.

## References

- ISIC Dataset: [Link to Dataset]
- TensorFlow Documentation: [Link to Documentation]

## Usage Instructions

To use this model, follow these steps:

1. Clone the repository: `git clone git clone https://github.com/vishnugamini/AdvancedDermatologicalSegmentation`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the model on your data

## Future Work

Future enhancements could include further optimizing the model for real-time processing, expanding the dataset to include more diverse skin types, and exploring additional architectural improvements.
