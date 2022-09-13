<img src="https://securaworld.com/wp-content/uploads/2018/11/solution11-1.jpg ">

### Helmet Detection

The primary safety equipment of motorcyclists is the helmet. The helmet protects the motorcyclist against accidents. Although helmet use is mandatory in many countries, some motorcyclists do not use or misuse them. Over the past years, many works have been carried out in traffic analysis, including vehicle detection, classification, and helmet detection. Intelligent traffic systems were implemented using computer vision algorithms, such as background and foreground image detection to segment the moving objects in the scene and image descriptors to extract features. Computational intelligence algorithms are used, too, like machine learning algorithms, to classify the objects. 


So, it is necessary to develop a system for automatically detecting helmet wearing for road safety using AI technique. Thus, a custom object detection model is created using a Machine learning-based algorithm that can detect Motorcycle riders.

### Implement

* Develop Python Implementation of Helmet Detection
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.


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
    #4. return output :output must be a json, which included output prediction. for example {"output":"SAVED FILE PATH WITH DETECTION"]}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  - type: image/Video
output:
  - type: image
main: main.ipynb
```