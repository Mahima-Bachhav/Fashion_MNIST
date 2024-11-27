#### Project Overview:
The **Fashion MNIST Classification Project** leverages the power of a **ResNet (Residual Network)** model to classify grayscale images from the Fashion MNIST dataset. This dataset contains 28x28 grayscale images of 10 different classes of fashion items such as shirts, shoes, bags, and coats. By utilizing ResNet, a deep convolutional neural network known for its ability to train effectively on complex datasets, the project aims to achieve high accuracy and robust predictions for fashion image classification tasks.

#### Key Features:
1. **Fashion MNIST Dataset**:
   - Contains **60,000 training images** and **10,000 test images** across 10 classes.
   - Each image is a **28x28 grayscale image** representing various fashion items.
   - Classes include: *T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, and Ankle Boot*.

2. **Model Architecture**:
   - **ResNet (Residual Network)** is employed to handle the classification task.
   - The input images are converted from grayscale (1 channel) to RGB (3 channels) to match ResNet's expected input format.
   - **Pretrained ResNet Weights**: A pretrained version of ResNet was used to accelerate training and improve model performance.
   - Fine-tuning: The final layers of the model were adapted for the Fashion MNIST dataset, ensuring compatibility with the 10 output classes.

3. **Preprocessing and Data Augmentation**:
   - Images are resized from **28x28** to **224x224** to match ResNet's input size.
   - Grayscale images are **duplicated into 3 channels** for compatibility with ResNet.
   - Normalization is applied to scale pixel values and improve training stability.

4. **Training and Validation**:
   - The model was trained using **PyTorch** with techniques like:
     - **Cross-entropy loss** for multi-class classification.
     - **Learning rate scheduling** to optimize the training process.
     - **Adam optimizer** for faster convergence.
   - **TQDM** progress bars were integrated to monitor training and validation progress.

5. **Evaluation**:
   - The model's accuracy and loss were evaluated on the test dataset.
   - Predictions were compared against ground truth, with visualizations highlighting correct and incorrect classifications.
   - Performance metrics like accuracy and loss were tracked


