# Traffic-AI

Traffic-AI is a deep learning project that utilizes TensorFlow and computer vision to recognize and classify road signs from digital images. This project is designed to help self-driving cars understand and interpret their environment by identifying various road signs such as stop signs, speed limit signs, yield signs, and more.

## Getting Started

To get started with Traffic-AI, follow these steps:

1. Clone the repository to your local machine:

   ```bash
   git clone https://github.com/roniboukheir1/Traffic-AI.git
   ```
2. Navigate to the project directory:
   ```bash
     cd Traffic-AI
     ```
3. Install the required dependencies
    ```bash
     pip install -r requirements.txt
     ```

## Usage

You can use Traffic-AI to train a neural network for recognizing road signs for images.
### Follow these steps:
  1. Organize the dataset: Place your road sign images in a directory structure where each category is represented in subdirectory(eg. 0,1,2 for different sign category)
  2. Run the training script:
      ```bash
        python traffic.py data_directory [model.h5]
      ``` 
  3. The script will load the data, split it into the training data and testing sets, and train a neural network model
  4. After training, the model will evaluate on the testing data, and you will see the evauluation results.

## Data 

Traffic-AI uses the German Traffic Sign Recognition Benchmark (GTSRB) dataset, which contains thousands of images of 43 different types of road signs. The data is organized into subdirectories, each representing a sign category.

## Model Architecture 

The neural network model used in Traffic-AI is designed to handle image inputs of shape (IMG_WIDTH, IMG_HEIGHT, 3), where IMG_WIDTH and IMG_HEIGHT are the desired image dimensions. The model consists of convolutional layers, max-pooling layers, dense layers, and dropout layers.

You can experiment with different model architectures by adjusting the code in the `get_model` function.

## Experimentation

During the development of Traffic-AI, we conducted experiments to fine-tune the model's performance. We explored various hyperparameters, such as the number of convolutional layers, filter sizes, pool sizes, and hidden layers.

## Contribution 

Contributions to Traffic-AI are welcome! If you have ideas for improvements or would like to add new features, please open an issue or submit a pull request.
