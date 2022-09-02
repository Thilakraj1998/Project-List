<img src="https://media.kairos.com/blog-images/crowd.png" height=550 width=1450>

## Face Detection

* Face detection also called facial detection is an artificial intelligence (AI) based computer technology used to find and identify human faces in digital images. 
* Face detection technology can be applied to various fields including security, biometrics, law enforcement, entertainment and personal safety to provide surveillance and tracking of people in real-time.
* Face detection has progressed from rudimentary computer vision techniques to advances in machine learning (ML) to increasingly sophisticated artificial neural networks (ANN) and related technologies; the result has been continuous performance improvements. 
* It now plays an important role as the first step in many key applications -- including face tracking, face analysis and facial recognition. Face detection has a significant effect on how sequential operations will perform in the application.

### Implement

Since Face Detection Problem has a wide variety of applicable Application in different domain and industries

* Develop Python Implementation of Face Detection
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.
* Output of face detection module should be saved in respective formats.

### Usage

* Create a separate ipynb file required for model prediction and usage of the model if you are utilising the custom-trained model. If the implementation doesn't require any AI or ML model training or uses a specialised library, avoid creating a separate training ipynb file.
* Create a function which will handle all the data preprocessing and engineering which is required to make prediction.

### Submission

To make a successful submission to the project repository, the following files have to be submitted:

* Training Code file(.ipynb):- AI/ML model training file for reproducibility of the results.
* Usage Code file(.ipynb):- A usage file to utilize the model for prediction/Recognition.
* Saved Model file(.h5/.pickle):- Saved Trained Model in appropriate/accepted format


### Note

In Usage, file creates a function main() accepting single input, which can either be an image or video. Through this function, other required functions to make detection should be called and return output in the appropriate format.

**Example**:
```
def main(input):
    data=data_preprocessing(input)
    output=model_prediction(data)
    return output
    
```