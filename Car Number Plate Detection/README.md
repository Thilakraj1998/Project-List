
<img src="https://miro.medium.com/max/1200/1*TWZM67eaCs0mMBFqs9HFBA.jpeg" height=450 width =1500>

### Car Number Plate Detection and Optical Character Recognition(OCR)

The massive integration of information technologies, under different aspects of the modern world, has led to the treatment of vehicles as conceptual resources in information systems. Since an autonomous information system has no meaning without any data, there is a need to reform vehicle information between reality and the information system. This can be achieved by human agents or by special intelligent equipment that will allow the identification of vehicles by their registration plates in real environments. Among intelligent equipment, mention is made of the system of detection and recognition of the number plates of vehicles. The system of vehicle number plate detection and recognition is used to detect the plates and then make the recognition of the plate that is to extract the text from an image and all that thanks to the calculation modules that use location algorithms, segmentation plate and character recognition. The detection and reading of license plates is a kind of intelligent system and it is considered because of the potential applications in several sectors which are quoted:

- Command force: This system is used for the detection of stolen and searched vehicles. The detected plates are compared to those of the reported vehicles.

- Parking management: The management of car entrances and exits.

- Road safety: This system is used to detect license plates exceeding a certain speed, coupling the plate reading system with road radar, crossing wildfires


### Implement

Since Car Number/License Plate Detection Problem has a wide variety of applicable Application in different domain and industries

* Develop Python Implementation of the follow problem to Detection and recognize License Plate Number
* Implementation should have the ability to infer Image files, video files, and video streams(webcams).
* Implementation should be easy to integrate with restful API frameworks.
* Output of detection module should be saved in respective formats.


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
    #4. return output :output must be a json, which included output prediction. for example {"output":"SAVED FILE PATH WITH DETECTION","prediction":[LIST OF DETECTED LICENSE NUMBERS]]}
    
```

### YAML Configuration:

Along with the above mentioned requirements and changes, include a YAML file which contains instruction for the execution of Usage file.

YAML file contain details regarding input format,output format, usage file name which included above mentioned main function.

**example :**

```
version: 1
input:
  type: image
output:
  type: image
requirement: requirement.txt
main: main.ipynb
```
**saved by name : blobcity.yaml**

Also include requirement.txt file in the submission with required version of the library mentioned in it.
