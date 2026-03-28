Plant Disease Segmentation is a deep learning project focused on accurately identifying and segmenting diseased regions in plant leaves using advanced image segmentation techniques. Built with Python, the project implements a baseline [U-Net](https://arxiv.org/abs/1505.04597) model alongside an enhanced version incorporating [BiFPN](https://arxiv.org/abs/1911.09070) for improved multi-scale feature fusion. The workflow covers data preprocessing, model training with optimization strategies like early stopping and learning rate scheduling, and evaluation using metrics such as Mean IoU, Dice coefficient, and pixel accuracy. It also includes visual comparisons of predictions to highlight performance differences, demonstrating how architectural improvements can significantly boost segmentation accuracy in real-world agricultural applications.

This project implements plant leaf disease segmentation using deep learning, also the models are trained and evaluated on a dataset of plant leaf images and corresponding segmentation masks.

## Project Structure

- `BIFPN_Segmentation.ipynb`: Notebook for U-Net with BiFPN model definition, training, and evaluation.
- `U-Net_Architecture.ipynb`: Baseline U-Net model training and evaluation.
- `Project_Comparison.ipynb`: Comparison and visualization of predictions from both models.

## Model Architectures

- **U-Net**: A standard encoder-decoder architecture for image segmentation.
- **U-Net with BiFPN**: Extends U-Net by integrating BiFPN for improved multi-scale feature fusion, enhancing segmentation accuracy.

## Key Features

- **Data Loading**: Images and masks are loaded and preprocessed to size 128x128.
- **Training**: Both models are trained with Adam optimizer, early stopping, and learning rate reduction callbacks.
- **Evaluation Metrics**: Mean IoU, Dice coefficient, and pixel accuracy are used for performance evaluation.
- **Visualization**: Side-by-side comparison of segmentation results on unseen images.

## Usage

1. **Requirements**
   - Python 3.x
   - TensorFlow
   - Keras
   - NumPy
   - OpenCV
   - scikit-learn
   - Matplotlib

2. **Training**
   - Run U-Net_Architecture.ipynb to train and save the baseline U-Net model.
   - Run BIFPN_Segmentation.ipynb to train and save the U-Net with BiFPN model.

3. **Comparison & Visualization**
   - Use Project_Comparison.ipynb to load both models and visualize predictions on unseen images.

## Results

- The U-Net with BiFPN generally achieves higher segmentation accuracy and better generalization on unseen images compared to the baseline U-Net.

## References

- [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597)
- [EfficientDet: Scalable and Efficient Object Detection](https://arxiv.org/abs/1911.09070) (BiFPN)

---

For more details, see the code and results in the provided notebooks.
