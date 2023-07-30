# Style&Wrap Recommender - README

## Description

The "Style&Wrap Recommender" is a web application that uses deep learning and machine learning techniques to recommend visually similar images based on the input image provided by the user. It leverages the ResNet50 pre-trained model for feature extraction and the Nearest Neighbors algorithm to find similar images.

## How it works

The application is built using the following technologies and libraries:

- **Python**: The core language used for coding the application.
- **TensorFlow**: The deep learning framework for building and training the image recognition model.
- **Streamlit**: The web application framework for creating the user interface.
- **NumPy**: A library used for numerical computing with Python.
- **PIL**: Python Imaging Library used to handle image files.

## Features

1. **Upload Image**: Users can upload an image they want to find similar images for.

2. **Recommendations**: Once the user uploads an image, the application extracts its features using the ResNet50 model. It then calculates the similarity between this image and the rest of the images in the dataset using the Nearest Neighbors algorithm. The top 5 visually similar images are displayed as recommendations.

## How to Use

1. Make sure you have Python installed on your system.

2. Install the required dependencies by running the following command:
   ```
   pip install tensorflow streamlit numpy pillow
   ```

3. Clone this repository to your local machine.

4. Download the pre-trained ResNet50 model weights and place them in the appropriate location:
   - Download the ResNet50 model from TensorFlow's official website or GitHub repository.
   - Place the downloaded model weights file in the same directory as the application code.

5. Prepare your dataset:
   - Place the images you want to use for similarity comparison in the 'images' directory.

6. Run the feature extraction script:
   - Open a terminal and navigate to the project directory.
   - Execute the following command to extract features from the images and save them in 'embeddings.pkl' and 'filenames.pkl':
     ```
     python feature_extraction.py
     ```

7. Run the Streamlit app:
   - Open a terminal and navigate to the project directory.
   - Execute the following command to launch the web application:
     ```
     streamlit run app.py
     ```

8. Access the application in your web browser by visiting the URL displayed in the terminal after running the Streamlit app.

9. Upload an image and view the recommended visually similar images.

## Note

Please note that the application relies on the ResNet50 model for feature extraction, which requires significant computational resources. If you encounter performance issues, consider running the application on a system with a powerful GPU.

## Credits

This application was developed by Vansh Malhotra as part of my E-commerce Website Project . It builds upon the work of the TensorFlow team for the ResNet50 model and the Streamlit development team for the web application framework.

For any questions or issues, feel free to contact vanshmalhotra353@gmail.com

