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

Input must be either URL to the Image/video. if URL is passed then, download the video file into the local directory, else read from the given path.

```
def main(input=URL):  
    """
      param1: String : URL for the image/video file.

      return: JSON : output of the model prediction

    """
    #perform following tasks:
    #1. checks for validate URL and download file into the working directory,uses the downloaded file path.
    #2. perform preprocessing on the data.
    #3. perform prediction on the given data and produce respective output
    #4. return output :output must be a json, which included output prediction. for example {"output":"SAVED FILE PATH WITH DETECTION","prediction":{"Faces":Count}]]}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: image
output:
  - type: image
main: main.ipynb
```